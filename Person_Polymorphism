using System;

// Base Class
public class Person
{
    public string Name { get; set; }
    public string Email { get; set; }

    public Person(string name, string email)
    {
        Console.WriteLine("Person Constructor Called");
        Name = name;
        Email = email;
    }

    public void DisplayBasicInfo()
    {
        Console.WriteLine($"Name: {Name}, Email: {Email}");
    }
}

// Derived Class 1
public class Student : Person
{
    public string StudentId { get; set; }
    public double GPA { get; set; }

    public Student(string name, string email, string studentId, double gpa) : base(name, email)
    {
        Console.WriteLine("Student Constructor Called");
        StudentId = studentId;
        GPA = gpa;
    }
}

// Derived Class 2
public class Employee : Person
{
    public string EmployeeId { get; set; }
    public double Salary { get; set; }

    public Employee(string name, string email, string employeeId, double salary) : base(name, email)
    {
        Console.WriteLine("Employee Constructor Called");
        EmployeeId = employeeId;
        Salary = salary;
    }
}

// Derived Class 3 (Inherits from Employee)
public class Teacher : Employee
{
    public string CourseName { get; set; }

    public Teacher(string name, string email, string employeeId, double salary, string courseName) 
        : base(name, email, employeeId, salary)
    {
        Console.WriteLine("Teacher Constructor Called");
        CourseName = courseName;
    }

    public void Teach()
    {
        Console.WriteLine($"{Name} is teaching {CourseName}.");
    }
}

class Program
{
    static void Main()
    {
        Console.WriteLine("--- Creating Student ---");
        Student student = new Student("Ali", "ali@mail.com", "S1234", 3.8);
        student.DisplayBasicInfo();

        Console.WriteLine("\n--- Creating Teacher ---");
        Teacher teacher = new Teacher("Dr. Ahmed", "ahmed@mail.com", "E987", 5000, "OOP C#");
        teacher.DisplayBasicInfo();
        teacher.Teach();
    }
}
