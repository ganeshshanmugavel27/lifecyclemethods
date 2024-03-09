# Ex.No:2 To create a HelloWorld Activity using all lifecycles methods to display messages.


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

/*
Program to print the text “Hello World”.
Developed by:GANESH S
Registeration Number :212222040042
*/
## ACTIVITY_MAIN.XML
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#EDE177"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/app_name"
        android:textColor="#F40B0B"
        android:textSize="40sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
## MAINACTIVITY.JAVA
```
package com.example.lifecycle;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Toast.makeText(getApplicationContext(), "OnCreate called", Toast.LENGTH_LONG).show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnStart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart(){
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnRestart called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "OnStop called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "OnPause called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "OnDestroy called", Toast.LENGTH_LONG);
        toast.show();
    }
}
```
## OUTPUT
![Screenshot 2024-03-09 112805](https://github.com/ganeshshanmugavel27/lifecyclemethods/assets/122046208/b539d629-d054-4379-a561-5218b4982440)
![MAD EX02 2](https://github.com/ganeshshanmugavel27/lifecyclemethods/assets/122046208/3fc14b64-facf-47df-aeb2-af6f71619c22)
![WhatsApp Image 2024-03-09 at 11 28 13_b566a184](https://github.com/ganeshshanmugavel27/lifecyclemethods/assets/122046208/6a5ac46f-6abe-4a67-887b-1c210fa18d0e)
![WhatsApp Image 2024-03-09 at 11 28 37_df0bd06b](https://github.com/ganeshshanmugavel27/lifecyclemethods/assets/122046208/0e28bbb8-0759-46f1-96e2-95c352cf1ebc)
![WhatsApp Image 2024-03-09 at 11 28 50_7e842c7d](https://github.com/ganeshshanmugavel27/lifecyclemethods/assets/122046208/6cfe4f93-6193-4e99-83f6-e7481baad713)
![WhatsApp Image 2024-03-09 at 11 28 25_4b5e4268](https://github.com/ganeshshanmugavel27/lifecyclemethods/assets/122046208/a6ff9d2c-ba04-4c52-9144-b940d3759255)





## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
