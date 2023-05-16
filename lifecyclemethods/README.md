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
   ## XML
   ![xml](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/36e4861c-28d7-4c8f-8c31-204ec0fafcff)
   ## MAIN
   ![main](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/b9e2d4ff-3693-4756-9bb7-733f792d1326)
   ## ON_CREATE()
   ![crt](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/8d10797d-085e-4f19-af60-3b301593e0f7)
   ## ON_START()
   ![strt](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/808f60d1-3452-45ee-9218-76498727409e)
   ## ON_RESUME()
   ![resum](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/5d122070-2879-4980-8fb5-7de97c5b65ff)
   ## ON_PAUSE()
   ![pas](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/de9d30b5-1169-46db-b579-d41164280a0f)
   ## ON_STOP()
   ![stp](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/a92a6341-24e3-4d5c-bb13-b0ddff7a83a7)
   ## ON_RESTART()
   ![res](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/89b41d12-373f-4bca-abdf-4131c97d2726)
   ## ON_DESTROY()
   ![des](https://github.com/HariHaranLK/Mobile-Application-Development/assets/132996089/d2ab9043-e633-4992-b72e-f8f604910043)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
