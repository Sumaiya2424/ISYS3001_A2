# ISYS3001_A2
//Entity
public class Student{
  private String contactNumber;
  
  //getter and setter methods
  


    public String getContactNumber() { return contactNumber; }
    public void setContactNumber(String contactNumber) { this.contactNumber = contactNumber; }
	
	//student repository
	

   package com.studentinfo.repository;
   
   import com.studentinfo.model.Student;
   
   public interface StudentRepository extends JpaRepository<Student, String> {
}
   
   
   
