```mermaid
\begin{center}
\begin{tikzpicture}[scale=1.5]
% Отрисовка атомов бериллия
\node[circle, fill=blue!20, draw, inner sep=2pt] (Be1) at (0,0) {Be};
\node[circle, fill=blue!20, draw, inner sep=2pt] (Be2) at (3,0) {Be};

% Отрисовка мостиковых атомов хлора
\node[circle, fill=green!20, draw, inner sep=2pt] (ClB1) at (1.5, 1) {Cl};
\node[circle, fill=green!20, draw, inner sep=2pt] (ClB2) at (1.5, -1) {Cl};

% Отрисовка терминальных атомов хлора
\node[circle, fill=green!10, draw, inner sep=2pt] (ClT1) at (-1.5, 0) {Cl};
\node[circle, fill=green!10, draw, inner sep=2pt] (ClT2) at (4.5, 0) {Cl};

% Обычные ковалентные связи (терминальные)
\draw[thick] (Be1) -- (ClT1);
\draw[thick] (Be2) -- (ClT2);

% Мостиковые связи: сочетание ковалентной и донорно-акцепторной
% Модель 1: Хлор 1 донор для Be2, ковалентно связан с Be1
\draw[thick] (Be1) -- (ClB1);
\draw[->, >=stealth, ultra thick, blue] (ClB1) -- (Be2);

% Модель 2: Хлор 2 донор для Be1, ковалентно связан с Be2
\draw[thick] (Be2) -- (ClB2);
\draw[->, >=stealth, ultra thick, blue] (ClB2) -- (Be1);

% Подписи
\node at (1.5, 1.4) {Мостиковый Cl (Донор)};
\node at (1.5, -1.4) {Мостиковый Cl (Донор)};
\node at (-1.8, 0.3) {Терминальный Cl};
\node at (4.8, 0.3) {Терминальный Cl};
\end{tikzpicture}
\end{center}
```
