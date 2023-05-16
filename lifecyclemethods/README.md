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
   ![xml](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/d37d40f6-b9dd-4c0d-bc32-690242712987) <br>
   ![main](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/a4802684-e891-4287-99c3-939091c6a110) <br>
   ![crt](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/957f7f16-76d1-4031-800c-f8cafc7bf535) <br>
   ![strt](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/bf7c94c7-3701-4764-a27f-b1cad735a61d) <br>
   ![resum](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/600622b9-d723-45e9-9d3c-5930a77e9ef3) <br>
   ![pas](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/2a232c12-304e-4193-b970-44e7358cf81c) <br>
   ![stp](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/643cd6d5-b876-457d-a171-563b0acb154a) <br>
   ![res](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/4324cefd-da3f-4568-9c53-f7318a72a9a9) <br>
   ![des](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/1cc32493-8bdf-42c9-9a66-8d09b4015427) <br>


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
