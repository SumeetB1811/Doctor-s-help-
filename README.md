# Doctor-s-help-
Mini Project A.
<br>
Author - SUMEET BHAGAT

// Doctor's GUI
import java.awt.*;
import java.awt.event.*;
import javax.swing.*;

public class doc1 extends JFrame implements ActionListener {
    JPanel panel = new JPanel();
    
    Button b1 = new Button("Submit");
    Label l1 = new Label("Name:", Label.LEFT);
    Label l2 = new Label("Age:", Label.LEFT);
    Label l3 = new Label("Gender(M/F):", Label.LEFT);
    Label l4 = new Label("Address:", Label.LEFT);
    Label l5 = new Label("Specialization: ", Label.LEFT);
    Label l6 = new Label("Contact: ", Label.LEFT);
    Label l7 = new Label("Course :", Label.LEFT);
    Label l8 = new Label("Doctor's details: ", Label.CENTER);
    Label label = new Label();

    TextField t1 = new TextField();
    TextField t3 = new TextField();

    Choice c1 = new Choice();

    Checkbox ck1 = new Checkbox("Male", false);
    Checkbox ck2 = new Checkbox("Female", false);

    TextArea t2 = new TextArea(" ", 180, 90, TextArea.SCROLLBARS_VERTICAL_ONLY);

    Choice course = new Choice();
    Choice specialization = new Choice();
    Choice age = new Choice();

    public doc1() {
        setBackground(Color.red);
        setForeground(Color.black);
        setLayout(null);

        add(l1);
        add(l2);
        add(l3);
        add(l4);
        add(l5);
        add(l6);
        add(l7);
        add(l8);
        add(t1);
        add(t2);
        add(t3);
        add(ck1);
        add(ck2);

        add(course);
        add(specialization);
        add(age);
        add(b1);

        course.add("Select");
        course.add("M.B.B.S");
        course.add("B.M.S");
        course.add("B.Pharma");
        course.add("Ph.d");
        
        age.add("Select");
        age.add("17");
        age.add("18");
        age.add("19");
        age.add("20");
        age.add("21");
        age.add("22");
        age.add("23");
        age.add("24");
        age.add("25");
        age.add("26");
        age.add("27");
        age.add("28");
        age.add("29");
        age.add("30");
        age.add("31");
        age.add("32");
        age.add("33");
        age.add("34");
        age.add("35");
        age.add("36");
        age.add("37");
        age.add("38");
        age.add("39");
        age.add("40");
        age.add("41");
        age.add("42");
        age.add("43");
        age.add("44");
        age.add("45");
        age.add("45+");

        add(label);
        specialization.add("Select");
        specialization.add("Eye");
        specialization.add("Neorology");
        specialization.add("Ears");
        specialization.add("Physio");
        specialization.add("Skin");
        specialization.add("Bones");
        specialization.add("Muscles and tendons");
        specialization.add("Tongue");
        specialization.add("Cardiography");
        specialization.add("Lungs"); 
        
        l1.setBounds(25, 60, 90, 20);
        l2.setBounds(25, 85, 90, 20);
        l3.setBounds(25, 110, 90, 20);
        l4.setBounds(25, 145, 90, 20);
        l5.setBounds(25, 245, 90, 20);
        l6.setBounds(25, 295, 90, 20);
        l7.setBounds(25, 270, 90, 20);
        l8.setBounds(25, 35, 280, 20);
        
        t1.setBounds(120, 60, 180, 20);
        t2.setBounds(120, 145, 180, 75);
        t3.setBounds(120, 295, 180, 20);

        ck1.setBounds(120, 110, 50, 20);
        ck2.setBounds(170, 110, 60, 20);

        
        age.setBounds(120, 85, 90, 20);
        specialization.setBounds(120, 245, 90, 20);
        course.setBounds(120, 270, 90, 20);
        b1.setBounds(120, 350, 65, 30);
        label.setBounds(140, 400, 90, 50);
        b1.addActionListener(this);
    }

    public void actionPerformed(ActionEvent ae) {
        if (ae.getActionCommand().equals("Submit")) {
            label.setText("Data is saved");
        }
    }
    
    public static void main(String args[]) {
        doc1 stu = new doc1();
        stu.setSize(500, 500);
        stu.setTitle("Doctor's Registration");
        stu.setVisible(true);
    }
}

// Patient's GUI
import java.awt.*;
import java.awt.event.*;

public class PATIENT extends Frame implements ActionListener {
    Button b1 = new Button("Submit");
    Label l1 = new Label("Name:", Label.LEFT);
    Label l2 = new Label("Age:", Label.LEFT);
    Label l3 = new Label("Gender(M/F):", Label.LEFT);
    Label l4 = new Label("Address:", Label.LEFT);
    Label l5 = new Label("Health Issues: ", Label.LEFT);
    Label l6 = new Label("Condition: ", Label.LEFT);
    Label l7 = new Label("Any prescribtions : ", Label.LEFT);
    Label l8 = new Label("Patient's details: ", Label.CENTER);
    Label l9 = new Label("Contact details : ", Label.LEFT);
    Label l10 = new Label("used before ", Label.LEFT);
    Label label = new Label();

    TextField t1 = new TextField();
    TextField t3 = new TextField();
    TextField t4 = new TextField();

    Choice c1 = new Choice();

    CheckboxGroup cbg = new CheckboxGroup();

    Checkbox ck1 = new Checkbox("Male", false, cbg);
    Checkbox ck2 = new Checkbox("Female", false, cbg);

    Checkbox ck3 = new Checkbox("Headache", false, cbg);
    Checkbox ck4 = new Checkbox("Stomachache", false, cbg);
    Checkbox ck5 = new Checkbox("Fever", false, cbg);
    Checkbox ck6 = new Checkbox("Cough", false, cbg);
    Checkbox ck7 = new Checkbox("Joint Pain ", false, cbg);
    Checkbox ck8 = new Checkbox("Running Nose", false, cbg);
    Checkbox ck9 = new Checkbox("Giddiness", false, cbg);
    Checkbox ck10 = new Checkbox("Nausea", false, cbg);
    Checkbox ck11 = new Checkbox("Diarrhea", false, cbg);
    Checkbox ck12 = new Checkbox("Itchy skin.", false, cbg);
    Checkbox ck13 = new Checkbox("Dark urine color.", false, cbg);
    Checkbox ck14 = new Checkbox("Swelling in the legs and ankles.", false, cbg);
    Checkbox ck15 = new Checkbox("Pale stool color.", false, cbg);
    Checkbox ck16 = new Checkbox("Skin and eyes that appear yellowish ", false, cbg);
    Checkbox ck17 = new Checkbox("Blood in your urine.", false, cbg);
    Checkbox ck18 = new Checkbox("Burning feeling when you urinate.", false, cbg);
    Checkbox ck19 = new Checkbox("Redness in eye.", false, cbg);
    Checkbox ck20 = new Checkbox("Swelling of eyelids.", false, cbg);
    Checkbox ck21 = new Checkbox("Chest pain that may feel like pressure, tightness, pain, squeezing or aching.", false, cbg);
    Checkbox ck22 = new Checkbox("Cold sweat.", false, cbg);
    Checkbox ck23 = new Checkbox("Shortness of breath.", false, cbg);
    
    Checkbox ck24 = new Checkbox("Normal", false, cbg);
    Checkbox ck25 = new Checkbox("Urgent", false, cbg);
    Checkbox ck26 = new Checkbox("Almost there", false, cbg);
    
    TextArea t2 = new TextArea(" ", 180, 90, TextArea.SCROLLBARS_VERTICAL_ONLY);

    Choice age = new Choice();

    public PATIENT() {
        setBackground(Color.red);
        setForeground(Color.black);
        setLayout(null);

        add(l1);
        add(l2);
        add(l3);
        add(l4);
        add(l5);
        add(l6);
        add(l7);
        add(l8);
        add(l9);
        add(l10);

        add(t1);
        add(t2);
        add(t3);
        add(t4);

        add(ck1);
        add(ck2);
        add(ck3);
        add(ck4);
        add(ck5);
        add(ck6);
        add(ck7);
        add(ck8);
        add(ck9);
        add(ck10);
        add(ck11);
        add(ck12);
        add(ck13);
        add(ck14);
        add(ck15);
        add(ck16);
        add(ck17);
        add(ck18);
        add(ck19);
        add(ck20);
        add(ck21);
        add(ck22);
        add(ck23);

        add(ck24);
        add(ck25);
        add(ck26);

        add(age);
        add(b1);
        
        age.add("Select");
        age.add("17");
        age.add("18");
        age.add("19");
        age.add("20");
        age.add("21");
        age.add("22");
        age.add("23");
        age.add("24");
        age.add("25");
        age.add("26");
        age.add("27");
        age.add("28");
        age.add("29");
        age.add("30");
        age.add("31");
        age.add("32");
        age.add("33");
        age.add("34");
        age.add("35");
        age.add("36");
        age.add("37");
        age.add("38");
        age.add("39");
        age.add("40");
        age.add("41");
        age.add("42");
        age.add("43");
        age.add("44");
        age.add("45");
        age.add("45+");

        add(label);
        
        l1.setBounds(25, 60, 90, 20);
        l2.setBounds(25, 85, 90, 20);
        l3.setBounds(25, 110, 90, 20);
        l4.setBounds(25, 145, 90, 20);
        l5.setBounds(25, 245, 90, 20);
        l6.setBounds(25, 420, 90, 20);
        l7.setBounds(25, 445, 90, 20);
        l8.setBounds(25, 35, 280, 20);
        l9.setBounds(25, 495, 90, 20);
        l10.setBounds(25, 470, 90, 20);

        t1.setBounds(120, 60, 180, 20);
        t2.setBounds(120, 145, 180, 75);
        t3.setBounds(120, 445, 180, 50);
        t4.setBounds(120, 495, 180, 20);

        ck1.setBounds(120, 110, 50, 20);
        ck2.setBounds(170, 110, 60, 20);
        
        ck3.setBounds(120, 245, 60, 20);
        ck4.setBounds(220, 245, 60, 20);
        ck5.setBounds(320, 245, 60, 20);
        ck6.setBounds(120, 270, 60, 20);
        ck7.setBounds(220, 270, 60, 20);
        ck8.setBounds(320, 270, 60, 20);
        ck9.setBounds(120, 295, 60, 20);
        ck10.setBounds(220, 295, 60, 20);
        ck11.setBounds(320, 295, 60, 20);
        ck12.setBounds(120, 320, 60, 20);
        ck13.setBounds(220, 320, 60, 20);
        ck14.setBounds(320, 320, 60, 20);
        ck15.setBounds(120, 345, 60, 20);
        ck16.setBounds(220, 345, 60, 20);
        ck17.setBounds(320, 345, 60, 20);
        ck18.setBounds(120, 370, 60, 20);
        ck19.setBounds(220, 370, 60, 20);
        ck20.setBounds(320, 370, 60, 20);
        ck21.setBounds(120, 395, 60, 20);
        ck22.setBounds(220, 395, 60, 20);
        ck23.setBounds(320, 395, 60, 20);

        ck24.setBounds(120, 420, 60, 20);
        ck25.setBounds(220, 420, 60, 20);
        ck26.setBounds(320, 420, 60, 20);

        
        age.setBounds(120, 85, 90, 20);
        b1.setBounds(120, 550, 65, 30);
        label.setBounds(140, 700, 90, 50);
        b1.addActionListener(this);
    }

    public void actionPerformed(ActionEvent ae) {
        if (ae.getActionCommand().equals("Submit")) {
            label.setText("Data is saved");
        }
    }

    public static void main(String args[]) {
        PATIENT stu = new PATIENT();
        stu.setSize(500, 500);
        stu.setTitle("Patient's Registration");
        stu.setVisible(true);
    }
}
