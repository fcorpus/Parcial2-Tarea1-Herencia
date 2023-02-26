# Parcial2-Tarea1-Herencia
Parcial 2 Tarea 1 Herencia; 26/02/2023
@startuml


class Person{
  - String name;
  - LocalDate birthday;
 
 
  + getName(): String;
  + setName(String name);
 
  + getBirthday(): LocalDate;
  + setBirthday(LocalDate birthday);
}

class Employee extends Person {
  - String rpe;
 
  + getRpe(): String;
  + setRpe(String rpe);
}

class Student extends Person {
 
  - String code;
 
  + getCode(): String;
  + setCode(String code);
 
}

class Professor extends Employee  {

}


class Concierge extends Employee{


}

class AdministrativePerson  extends Employee{
}


class ScholarshipHolder  extends Employee {
  - String code;
 
  + getCode(): String;
  + setCode(String code);
}

@enduml








(![image](https://user-images.githubusercontent.com/123425340/221430851-b973503c-22b4-423f-8820-d8d00b6d13ab.png)
)
Herncia multiple es cuando una clase puede heredar de multiples clases.
Este tipo de herencia no es posible en java para evitar la ambigüedad en el codigo, hacerlo mas sencillo y porque puede que cree mas problemas de los que soluciona.
