# Java_Developer_Job_Post
#Developed by Mohamed El-Feky
#Used as a Job post for 3D|Diagnostix looking for a Java Developer
#Last edit was June 28 , 2016
public class TalentRequired {

    public enum Essentials {
        JavaSE,JavaEE,HTML,CSS,SQL
    };
    
    public enum Prefared {
        XML,JavaScript,JQuery,GWT,Vaadin,MySQL
    };
    public enum Knowledge {
        WebService,ORM,OOP,Design_Patterns,Application_Design
    };
    
    public static void main(String[] args) {
        
        TalentRequired talent = new TalentRequired();
        if(talent.gotEssentials() && talent.gotKnowledgeSet()){
            
            if(talent.gotPrefared()){
                
                if(talent.getMinimumExperiance() >1 && talent.getMinimumExperiance() <5)
                    
                    if(talent.sendCV())System.out.println("Hello 3D | Diagnostix");
            }
        } 
        
        
    }
    public boolean sendCV(){
        //Kindly Send us your C.v to 
        String mail = "recruitment@3ddx.com";
        return true;
    }
    
    public int getMinimumExperiance(){
        int minimumExp = 0;//change to your actual Minimum Experiance
        return minimumExp;
    }
    
    public boolean gotEssentials(){
        //DO you have Essentian Requirements for the Job
        boolean essentials = false;//change to true if you do 
        return essentials;
    }
    
    public boolean gotPrefared(){
        //DO you have Prefared  Requirements for the Job
        boolean prefared = false;//change to true if you have at least one 
        return prefared;
    }
    
    public boolean gotKnowledgeSet(){
        //DO you have Those Knowledge Set for the Job
        boolean iGotKnowledge = false;//change to true if you do 
        return iGotKnowledge;
    }
    
}
