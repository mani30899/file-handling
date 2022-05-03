# file-handling
java file handling
import java.io.File;
import java.io.IOException;
import java.io.FileWriter;
 class Mani{
     public static void main(String[]args){
		 File f=new File("TVS.txt");
		 boolean b=false;
		 FileWriter fw=null;
		 try{
		 b=f.createNewFile();
		 }catch(IOException e){
			 System.out.println(e);
		 }
        System.out.println(b);
		try{
			fw=new FileWriter(f);
		}catch(IOException e){
			System.out.println(e);
		}
		try{
			fw.write("Mani");
		}catch(IOException e){
			System.out.println(e);
		}
		try{
			fw.close();
		}catch(IOException e){
			System.out.println(e);
		}
	 }
 }  
