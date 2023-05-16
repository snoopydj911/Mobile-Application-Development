# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: Hari Haran L K
Registeration Number :212221040051
*/
```
**XML FILE:**
    
    
    <?xml version="1.0" encoding="utf-8"?>
    <androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="298dp"
        android:layout_height="90dp"
        android:layout_marginBottom="341dp"
        android:text="ACTIVITY CYCLE"
        android:textColor="@color/teal_200"
        android:textSize="36sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.588"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/imageView"
        app:layout_constraintVertical_bias="0.499" />

    <ImageView
        android:id="@+id/imageView"
        android:layout_width="92dp"
        android:layout_height="91dp"
        android:layout_marginBottom="32dp"
        android:src="@drawable/img"
        app:layout_constraintBottom_toTopOf="@+id/textView"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.498"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        tools:srcCompat="@tools:sample/avatars" />
        </androidx.constraintlayout.widget.ConstraintLayout>
        
**MAINACTIVITY:**
    
    package com.example.activity_cycle;
    import androidx.appcompat.app.AppCompatActivity;
    import android.os.Bundle;
    import android.widget.Toast;

    public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(),"Oncreate",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(),"Onstart",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(),"Onpause",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(),"onResume",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(),"OnStop",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected  void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(),"onDestroy",Toast.LENGTH_SHORT);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(),"onRestart",Toast.LENGTH_SHORT);
        toast.show();
    }
    }


## OUTPUT
   ![xml](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/87f3a213-a6ca-4f4e-ab4f-50fb865588ac) <br>
   ![main](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/88157ada-0f43-4851-8377-833b8e4074a6) <br>
   ![crt](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/5a3239ed-ecfe-47bc-86e4-eecf45ea03ad) <br>
   ![strt](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/8757021d-ab85-4fe2-8cf6-9aeff41d7e52) <br>
   ![resum](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/69ccd14f-999b-4879-8436-8c6c05074048) <br>
   ![pas](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/55d07c84-8ebb-4bf4-ba22-fc649e8e14df) <br>
   ![stp](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/8989f4ba-f9d7-4003-ab59-53c44342f978) <br>
   ![res](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/1ac2fe13-042c-4824-bac1-9c0ff6088593) <br>
   ![des](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/b7fddcc8-e2ef-4c22-bcca-d92572cf143b) <br>

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
