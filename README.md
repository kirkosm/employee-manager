# Employee Manager – Backend (Spring Boot)

Backend REST εφαρμογή διαχείρισης εργαζομένων με χρήση Java, Spring Boot και PostgreSQL.

## Τεχνολογίες

- Java 24+
- Spring Boot 3+
- Spring Data JPA
- PostgreSQL
- Maven
- CORS enabled

## Λειτουργίες

- Ανάγνωση (GET) όλων των εργαζομένων
- Δημιουργία (POST) νέου εργαζομένου
- Ενημέρωση (PUT) υπαρχόντων
- Διαγραφή (DELETE) με βάση ID
- Συνδέεται με React frontend μέσω REST API

## Δομή API

| Μέθοδος | Endpoint               | Περιγραφή                 |
|--------|------------------------|---------------------------|
| GET    | `/employees`           | Επιστρέφει όλους          |
| POST   | `/employees`           | Προσθήκη νέου             |
| PUT    | `/employees/{id}`      | Ενημέρωση υπάρχοντος      |
| DELETE | `/employees/{id}`      | Διαγραφή εργαζομένου      |

## Εκτέλεση τοπικά

1. Άνοιξε το έργο με IntelliJ
2. Βεβαιώσου ότι η βάση PostgreSQL τρέχει
3. Άλλαξε τα στοιχεία της DB στο `application.properties` αν χρειάζεται
4. Τρέξε το `EmployeeManagerApplication.java`

## Βάση Δεδομένων

Πίνακας `employees` με πεδία:

- id (Long)
- firstName (String)
- lastName (String)
- email (String)

## Σύνδεση με Frontend

Το React frontend κάνει αιτήματα στο `http://localhost:8080/employees`
