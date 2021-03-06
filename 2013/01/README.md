# Нормализация на пътища

След като се запознахме с основите на езика, нека използвайки само тях, да си имплементираме една проста функция, която да ни oпрости живота. Функцийката трябва да приема string, описващ път в операционната система, и да го опростява така, че да е разбираем от човек (или програмист).

Примерни входящи данни както следва:

"D/go/code/../src/warcluster/tests/first/../../"

"python/movies/episode1/../../lectures/lecture1/examples/../code/../../../mostImportant/MonthyPython/quotes/.."

Имплементирайте функция `parsePath`, която взема пътя като string. Функцията трябва да намери всичко комплекти от /директория + /.. и да ги премахне.
Върнатият резултат трябва да е string, съдържащ опростения път.

За пълнота, ще допълним, че текущата ви директория е "/" и е най-ниската в йерархията.
Т.е входящи пътища гласящи: "/", "./..", ".." и "../" се нормализират до "/" (текущата директория).

## Примери:

	>>> parsePath("D/go/code/../src/warcluster/tests/first/../../")
	/D/go/src/warcluster/

	>>> parsePath("/python/movies/episode1/../../lectures/lecture1/examples/../code/../../../mostImportant/MonthyPython/quotes/..")
	/python/mostImportant/MonthyPython/
