# ISYS3001_A2
//Entity
public class Unit{
  private String unitName;
  private String unitId;

  
  //getter and setter methods
  


    public String getUnitName() { return unitName; }
    public void setName(String unitName) { this.name = unitName; }


    public String getUnitId() { return unitId; }
    public void setName(String unitId) { this.name = unitId; }

	//Unit repository
	

   package com.unitinfo.repository;
   
   import com.unitinfo.model.Unit;
   
   public interface UnitRepository extends JpaRepository<Unit, String> {
}
   
   
   
