# ISYS3001_A2

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
   
