package com.studentinfo;

public class StudentInfo{
public static void main(String[] args){
   StudentNote.run(StudnetInfo.class, args);
   }
 }
 
 
 // Student catagories
 package com.studentinfo.catagories;
 
import javax.persistence.GeneratedValue;
import javax.persistence.GenerationType;
import javax.persistence.Entity;
import javax.persistence.Id;

//Entity
public class Student{
  private String name;
  private String id;
  private String contactNumber;
  
  //getter and setter methods
  
    public String getStudentId() { return studentId; }
    public void setStudentId(String studentId) { this.studentId = studentId; }

    public String getName() { return name; }
    public void setName(String name) { this.name = name; }

    public String getContactNumber() { return contactNumber; }
    public void setContactNumber(String contactNumber) { this.contactNumber = contactNumber; }
	
	//student repository
	

   package com.studentinfo.repository;
   
   import com.studentinfo.model.Student;
   
   public interface StudentRepository extends JpaRepository<Student, String> {
}
   
   
   
   
<!DOCTYPE html>
<html xmlns:th="UTL University">
<head>
    <title>Add Student</title>
</head>
<body>
    <h1>Add Student</h1>
    <form action="/add-student" method="post" th:object="${student}">
        <label>Student ID:</label><br/>
        <input type="text" th:field="*{studentId}" /><br/><br/>
        
        <label>Name:</label><br/>
        <input type="text" th:field="*{name}" /><br/><br/>
        
        <label>Contact Number:</label><br/>
        <input type="text" th:field="*{contactNumber}" /><br/><br/>
         
        <input type="submit" value="Add Student" />
    </form>
</body>
</html>
   
