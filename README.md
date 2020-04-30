# calculator
this is simple calculator app code example
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.example.a84.calculator.MainActivity">

    <RelativeLayout
        android:layout_width="368dp"
        android:layout_height="495dp"
        android:layout_marginBottom="8dp"
        android:layout_marginEnd="8dp"
        android:layout_marginTop="8dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent">

        <Button
            android:id="@+id/btn_1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignParentLeft="true"
            android:layout_alignParentStart="true"
            android:layout_below="@+id/edText1"
            android:layout_marginTop="60dp"
            android:onClick="PressOne"
            android:text="1"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_0"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_below="@+id/btn_8"
            android:layout_toEndOf="@+id/btn_7"
            android:layout_toRightOf="@+id/btn_7"
            android:text="0"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_9"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_below="@+id/btn_6"
            android:layout_toEndOf="@+id/btn_5"
            android:layout_toRightOf="@+id/btn_5"
            android:text="9"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_8"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_below="@+id/btn_5"
            android:layout_toEndOf="@+id/btn_7"
            android:layout_toRightOf="@+id/btn_7"
            android:text="8"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_7"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignLeft="@+id/btn_4"
            android:layout_alignStart="@+id/btn_4"
            android:layout_below="@+id/btn_4"
            android:text="7"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_6"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignBaseline="@+id/btn_5"
            android:layout_alignBottom="@+id/btn_5"
            android:layout_toEndOf="@+id/btn_5"
            android:layout_toRightOf="@+id/btn_5"
            android:text="6"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_5"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_below="@+id/btn_2"
            android:layout_toEndOf="@+id/btn_4"
            android:layout_toRightOf="@+id/btn_4"
            android:text="5"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_4"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignLeft="@+id/btn_1"
            android:layout_alignStart="@+id/btn_1"
            android:layout_below="@+id/btn_1"
            android:text="4"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_3"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignBaseline="@+id/btn_2"
            android:layout_alignBottom="@+id/btn_2"
            android:layout_toEndOf="@+id/btn_2"
            android:layout_toRightOf="@+id/btn_2"
            android:text="3"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignBaseline="@+id/btn_1"
            android:layout_alignBottom="@+id/btn_1"
            android:layout_toEndOf="@+id/btn_1"
            android:layout_toRightOf="@+id/btn_1"
            android:text="2"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_Add"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_above="@+id/btn_6"
            android:layout_alignParentEnd="true"
            android:layout_alignParentRight="true"
            android:backgroundTint="@android:color/darker_gray"
            android:text="+"
            android:textColor="@android:color/background_light"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_Sub"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignLeft="@+id/btn_Add"
            android:layout_alignStart="@+id/btn_Add"
            android:layout_below="@+id/btn_Add"
            android:backgroundTint="@android:color/darker_gray"
            android:text="-"
            android:textColor="@android:color/background_light"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_Mul"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignLeft="@+id/btn_Sub"
            android:layout_alignStart="@+id/btn_Sub"
            android:layout_below="@+id/btn_6"
            android:backgroundTint="@android:color/darker_gray"
            android:text="*"
            android:textColor="@android:color/background_light"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_Div"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignLeft="@+id/btn_Mul"
            android:layout_alignStart="@+id/btn_Mul"
            android:layout_below="@+id/btn_9"
            android:backgroundTint="@android:color/darker_gray"
            android:text="/"
            android:textColor="@android:color/background_light"
            android:textSize="18sp" />

        <EditText
            android:id="@+id/edText1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignParentEnd="true"
            android:layout_alignParentLeft="true"
            android:layout_alignParentRight="true"
            android:layout_alignParentStart="true"
            android:layout_alignParentTop="true"
            android:layout_marginTop="22dp"
            android:ems="10"
            android:inputType="textPersonName"
            android:textAlignment="textEnd"
            android:textSize="24sp" />

        <Button
            android:id="@+id/btn_calc"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_below="@+id/btn_0"
            android:layout_toEndOf="@+id/btn_0"
            android:layout_toRightOf="@+id/btn_0"
            android:backgroundTint="@android:color/holo_green_light"
            android:text="="
            android:textColor="@android:color/background_light"
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_dec"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_below="@+id/btn_7"
            android:layout_toLeftOf="@+id/btn_8"
            android:layout_toStartOf="@+id/btn_8"
            android:text="."
            android:textSize="18sp" />

        <Button
            android:id="@+id/btn_clear"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_alignParentEnd="true"
            android:layout_alignParentRight="true"
            android:layout_below="@+id/btn_Div"
            android:backgroundTint="@android:color/holo_blue_dark"
            android:text="clear"
            android:textColor="@android:color/background_light"
            android:textSize="18sp" />

    </RelativeLayout>
</android.support.constraint.ConstraintLayout>
