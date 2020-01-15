# CIS407-Java
Strayer Java Programming II

public class Artist {
   private String artistName;               //private fields
   private int birthYear,deathYear;
   public Artist()                   //default constructor
   {
       artistName="None";
       birthYear=0;
       deathYear=0;
   }
   public Artist(String artistName,int birthYear,int deathYear) //second constructor to initialize private fields
   {
       this.artistName=artistName;
       this.birthYear=birthYear;
       this.deathYear=deathYear;
   }
   public String getName()                         
   {
       return artistName;
   }
   public int getBirthYear()
   {                                               
       return birthYear;
   }
   public int getDeathYear()
   {                                               
       return deathYear;
   }
   public void printInfo()
   {                                    
       if(deathYear!=-1)
           System.out.println("Artist: "+artistName+" ("+birthYear+"-"+deathYear+")");      
       else
           System.out.println("Artist: "+artistName+", born "+birthYear);
   }
}
