#include <iostream>
#include <string>

using namespace std;

#pragma once
using namespace std;

struct Human
{
	int age;
	string name, surname;
};

struct Chool
{
	int nomer;
};

struct chobi
{

};

struct 
{

};

#include "ss.h"
#include "mystruct.h"




#include "funcPrintName.h"
#include "PrintAge.h"
#include "PrintChool.h"

#pragma once
#include <iostream>
using namespace std;
void printAge(int age);

#pragma once
#include <iostream>
using namespace std;
void chool(int nomer);

#pragma once
#include <string>
#include <iostream>
using namespace std;
void pringName(string name, string surname);
#include "funcPrintName.h"

#include "PrintChool.h"

void chool(int nomer)
{
	cout << "Номер школы: " << nomer << endl;
}

#include "PrintAge.h"

void printAge(int age)
{
	cout << "Возраст человека: " << age << endl;
}

void pringName(string name, string surname)
{
	cout << "Имя и фамилия человека: " << (name + " " + surname) << endl;
}


int main()
{
	setlocale(LC_ALL, "ru");
	Chool c1{ 476 };
	Human h1{ 14,"Шляхтин","Вова" };
	pringName(h1.name, h1.surname);
	printAge(h1.age);
	chool(c1.nomer);

	return 0;
}

