import java.util.ArrayList;

// 1. Vytvoření třídy Clazz
class Clazz {
    String name;
    ArrayList<Student> students = new ArrayList<>(); // 7. Přidejte atribut studenti do třídy Clazz

    // Konstruktor pro třídu Clazz
    public Clazz(String name) {
        this.name = name; // 2. Třída má atribut název
    }
}

// 4. Vytvoření třídy Student
class Student {
    String firstName;
    String lastName;
    int age;
    String className;

    // Konstruktor pro třídu Student
    public Student(String firstName, String lastName, int age, String className) {
        this.firstName = firstName;
        this.lastName = lastName;
        this.age = age;
        this.className = className; // 10. Nastavení atributu název třídy pro studenty
    }
}

// Hlavní třída
public class Main {
    public static void main(String[] args) {
        // 8. Vytvoření dvou tříd a 10 studentů
        Clazz classA = new Clazz("classA");
        Clazz classB = new Clazz("classB");

        for (int i = 1; i <= 10; i++) {
            // 9. Rozdělení studentů do tříd podle věku
            String className = (i <= 5) ? "classA" : "classB";
            int age = (i <= 5) ? i + 12 : i + 10;

            // Vytvoření nového studenta
            Student student = new Student("Student" + i, "Lastname" + i, age, className);

            // Přidání studenta do příslušné třídy
            if (className.equals("classA")) {
                classA.students.add(student);
            } else {
                classB.students.add(student);
            }
        }

        // 11. Výpis studentů do konzole
        for (Student studentA : classA.students) {
            System.out.println(studentA.firstName + " " + studentA.lastName + " " + studentA.className);
        }

        for (Student studentB : classB.students) {
            System.out.println(studentB.firstName + " " + studentB.lastName + " " + studentB.className);
        }
    }
}
