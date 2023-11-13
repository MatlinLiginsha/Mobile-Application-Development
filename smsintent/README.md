
# Ex.No:6 Design an android application Send SMS using Intent.


## AIM:

To create and design an android application Send SMS using Intent using Android Studio.

## EQUIPMENTS REQUIRED:

Android Studio(Latest Version)

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as smsintent and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Send SMS and Display details give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to create and design an android application Send SMS using Intent.
Developed by:
Registeration Number :
*/
```
## activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <ListView
        android:id="@+id/simpleListView"
        android:layout_width="335dp"
        android:layout_height="672dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
```
## MainActivity.java:
```
Package com.example.listimage;
import androidx.appcompat.app.AppCompatActivity;
import android.app.Activity;
import android.os.Bundle;
import android.widget.ListAdapter;
import android.widget.ListView;
public class MainActivity extends AppCompatActivity {
        ListView simpleList;
        String countryList[]={"India","China","australia","Portugle","America","NewZealand"};
        int flags[] = {R.drawable.india, R.drawable.china, R.drawable.australia, R.drawable.portugle, R.drawable.america,R.drawable.newzealand};
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        simpleList=(ListView)findViewById(R.id.simpleListView);
        CustomAdapter customAdapter=new CustomAdapter(gpetApplicationContext(),countryList,flags);
        simpleList.setAdapter((ListAdapter) customAdapter);
    }
}
```
## OUTPUT
![image](https://github.com/MatlinLiginsha/Mobile-Application-Development/assets/143495913/a553f746-a551-43b0-bee3-7171b9972a79)
## RESULT
Thus a Simple Android Application create and design an android application Send SMS using Intent using Android Studio is developed and executed successfully.
