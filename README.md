# Date: 22-08-2024
# BASIC-ANDROID-EX01-Implementation of a Hello world Activity using all lifecycles methods using Android Studio.
## AIM:
To create Hello world Activity using all lifecycles methods to display messages using android studio.
## EQUIPMENTS REQUIRED:
Android Studio(Min. required Artic Fox)
## ALGORITHM:
Step 1: Open Android Stdio and then click on File -> New -> New project.
Step 2: Then type the Application name as HelloWorld and click Next.
Step 3: Then select the Minimum SDK as shown below and click Next.
Step 4: Then select the Empty Activity and click Next. Finally click Finish.
Step 5: Design layout in activity_main.xml.
Step 6: Display message give in MainActivity file.
Step 7: Save and run the application.
## PROGRAM
DEVELOPED BY : Subalakshmi V
REGISTER NO: 212222040162
# MainActivity.java:
```
package com.example.helloworld;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart(){
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onResume(){
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onPause(){
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStop(){
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(),"OnStop Executed",Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "OnRestart Executed", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onDestroy(){
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        toast.show();
    }}
```
## Activity_Main.XML:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## OUTPUT:
# OnCreate Executed:
<img src="https://github.com/user-attachments/assets/b7e42e66-2dc0-4158-a879-aaa4dd25de53" width=200>

# OnPause Executed:
<img src="https://github.com/user-attachments/assets/4e187497-08c0-4708-b8aa-13cf933c4fe6" width=200>

# OnResume Executed:
<img src="https://github.com/user-attachments/assets/2a9fbfe2-4058-4e7d-9d1d-c4e890598740" width=200>

# OnRestart Executed:
<img src="https://github.com/user-attachments/assets/aee59563-60c0-4428-a57b-2abddcf7efd8" width=200>

# OnStart Executed:
<img src="https://github.com/user-attachments/assets/30bd7952-4605-4736-bbe8-69ba04bbad7c" width=200>

## RESULT:
Thus a program to implement the various life cycles of an activity is written and successfully executed using Android Studio.
