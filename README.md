 class HelloWorld {
    String name;
    int regNo=0;
    double GPA;
    double CGPA;

    // Constructor
    public HelloWorld(String name, int regNo, double GPA, double CGPA) {
        this.name = name;
       regNo =genrateRegNumber();
       this.GPA = GPA;
        this.CGPA = CGPA;
    }
private string genrateRegNumber(){
regNo++;
return +regNo;}

    // display 
    public void displayInfo() {
        System.out.printf("Name:%s\n " + name);
        System.out.printf("Registration Number:%s\n " + regNo);
        System.out.printf("GPA:%f\n " + GPA);
        System.out.printf("CGPA:%f\n " + CGPA);
    }

    
    public static int getStudentCount() {
        
        return 1;  
    }

    public static void main(String[] args) {
        HelloWorld student = new HelloWorld("zuha zia ", 98, 3.6, 2.57);
        student.displayInfo();
        System.out.println("Student Count: " + getStudentCount());
    }
}
