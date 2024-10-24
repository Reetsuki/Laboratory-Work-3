\documentclass[14pt, a4paper]{article}
\usepackage{cmap}
\usepackage{mathtext}
\usepackage[T2A]{fontenc}
\usepackage[utf8]{inputenc}
\usepackage[english,russian]{babel}
\usepackage{indentfirst}

\usepackage[colorlinks=true, allcolors=blue]{hyperref}
\usepackage{listings}
\usepackage{xcolor}
\usepackage{hyperref}

\title{Работа с LaTeX. Лабораторная работа №3}
\author{Выполнил: Тарский Дмитрий Николаевич, М3115}
\date{Октябрь 2024}

\lstset{
  backgroundcolor=\color{white}, % Цвет фона
  basicstyle=\ttfamily\small,     % Шрифт
  breaklines=true,                 % Перенос строк
  numbers=left,                   % Нумерация строк
  numberstyle=\tiny\color{gray},   % Стиль нумерации
  keywordstyle=\color{blue},       % Стиль ключевых слов
  commentstyle=\color{green},      % Стиль комментариев
  stringstyle=\color{red}          % Стиль строк
}

\begin{document}
\maketitle
\begin{center}
Преподаватель: Хасан Карим Асадович
\end{center}

\newpage

\tableofcontents

\section{Общее описание решения}

\subsection{Математические формулы}

\subsubsection*{\textbf{Окружность / круг}}

Площадь: $S = {\pi}R^2$

Периметр: $P = 2{\pi}R$

\subsubsection*{\textbf{Квадрат}}

Площадь: $S = a^2$

Периметр: $P = 4a$

\subsection{Способ решения}

Создание файлов с расширением .py различных фигур с функциями вычисления площадей и периметров.

Подробнее в следующем разделе.

\section{Описание каждой функции с примерами вызова}

\subsection{Функция Circle}

\begin{lstlisting}[language=Python]

import math

def area(r):
    return math.pi * r * r

def perimeter(r):
    return 2 * math.pi * r

\end{lstlisting}

\subsubsection*{\textbf{Описание логики программы}}

Функция \textit{area(r)} возвращает площадь круга с радиусом \textit{r}. 
Функция \textit{perimeter(r)} возвращает длину окружности с радиусом \textit{r}.

\subsubsection*{\textbf{Примеры вызова}}

\begin{center}
    \begin{tabular}{| c | c | c | c |}
        \hline
        Номер теста & Входные данные & Выходные данные \textit{area(r)} & Выходные данные \textit{perimeter(r)}\\
        \hline
        Test 1 & 3 & 28.274333882308138 & 18.84955592153876 \\
        \hline
        Test 2 & 4 & 50.26548245743669 & 25.132741228718345 \\
        \hline
        Test 3 & 0 & 0.0 & 0.0 \\
        \hline
        Test 4 & 100 & 31415.926535897932 & 628.3185307179587 \\
        \hline
    \end{tabular}
\end{center}

\subsection{Функция Square}

\begin{lstlisting}[language=Python]

def area(a):
    return a * a


def perimeter(a):
    return 4 * a


\end{lstlisting}

\subsubsection*{\textbf{Описание логики программы}}

Функция \textit{area(a)} возвращает площадь квадрата со стороной \textit{a}. Функция 
\textit{perimeter(a)} возвращает периметр квадрата со стороной \textit{a}.

\subsubsection*{\textbf{Примеры вызова}}

\begin{center}
    \begin{tabular}{| c | c | c | c |}
        \hline
        Номер теста & Входные данные & Выходные данные \textit{area(a)} & Выходные данные \textit{perimeter(a)}\\
        \hline
        Test 1 & 1 & 1 & 4 \\
        \hline
        Test 2 & 6 & 36 & 24 \\
        \hline
        Test 3 & 0 & 0 & 0 \\
        \hline
        Test 4 & 101 & 10201 & 404 \\
        \hline
    \end{tabular}
\end{center}

\section{Общее описание библиотеки geometric.lib}

Библиотека \href{https://github.com/smartiqaorg/geometric_lib}{geometric.lib} удобна тем, что позволяет с помощью встроенных функций находить различные характеристики различных геометрических объектов, а именно площадь и периметр круга и квадрата.

\section{Ссылка на проект}

По этой \href{https://github.com/Reetsuki/Laboratory-Work-3/edit/main/LaboratoryWork3.tex}{ссылке} можно перейти на исходный код этого документа в LaTeX. Перейдите для большей наглядности в документ LaboratoryWork3.tex

\end{document}
