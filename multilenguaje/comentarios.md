


##Para compilar con Makefile 
pongo "make executable"

#f a f
muestra que hizo

gfortran -c f-main.f90 -o f-main_f90.o
gfortran -c f-sum.f90 -o f-sum_f90.o
gfortran f-main_f90.o f-sum_f90.o -o f-main.e

#c a c
gcc -c c-main.c -o c-main_c.o
gcc -c c-sum.c -o c-sum_c.o
gcc c-main_c.o c-sum_c.o -o c-main.e

#c++ a c++
g++ -c cpp-main.cpp -o cpp-main_cpp.o
g++ -c cpp-sum.cpp -o cpp-sum_cpp.o
g++ cpp-main_cpp.o cpp-sum_cpp.o -o cpp-main.e


#f llama a c
compilo la subfuncion c hasta binario (-c) ---> gcc -c c-sum.c -o c-sum.o
compilo el main hasta binario (-c) ---> gfortran -c f-main.f90 -o f-main_f90.o
ACÂ ESTÀ LA PAPA: HAY QUE DECIRLE AL CÓDIGO DE C QUE VA A SER LLAMADO POR UN PROGRAMA EN FORTRAM. PARA ESO, PONGO LOS _ (FORTRAM PONE ESO EN LAS FUNCIONES, ASI QUE HAY PONERSELO A C - DECORADORES-), Y ESCRIBO TODO CON PUNTEROS (OJO CON LAS ENTRADAS DE LA FUNCION, TMB HAY QUE CAMBIARLAS). DESPUÉS HAGO: 
gfortran f-main_f90.o c-sum.o -o f-main.e       ¿PODRÍA USAR GCC TAMBIÉN? ME PA QUE SÍ

