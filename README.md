<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <LinearLayout
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:orientation="vertical"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent">

        <TextView
            android:id="@+id/textView"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/hello_world" />

        <Button
            android:id="@+id/button"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/button_test" />

        <EditText
            android:id="@+id/editName"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:autofillHints="name"
            android:drawableStart="@android:drawable/ic_menu_edit"
            android:hint="@string/enter_name"
            android:inputType="textPersonName"
            android:maxLength="30"
            android:singleLine="true" />

        <ImageView
            android:id="@+id/imageProfile"
            android:layout_width="150dp"
            android:layout_height="150dp"
            android:adjustViewBounds="true"
            android:contentDescription="@string/profile_image_desc"
            android:scaleType="centerCrop"
            android:src="@drawable/profile_pic" />

        <CheckBox
            android:id="@+id/checkAgree"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:buttonTint="#2196F3"
            android:checked="false"
            android:text="@string/agree_term" />
        <RadioGroup
            android:id="@+id/genderGroup"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content">

            <RadioButton
                android:id="@+id/radioMale"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/male"
                android:checked="true"
                android:buttonTint="#FF5722" />

            <RadioButton
                android:id="@+id/radioFemale"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/female" />

        </RadioGroup>


        <ToggleButton
            android:id="@+id/toggleWifi"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:textOn="@string/wifi_on"
            android:textOff="@string/wifi_off"
            android:checked="false"
            android:backgroundTint="#4CAF50" />

        <androidx.appcompat.widget.SwitchCompat
            android:id="@+id/switchBluetooth"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/bluetooth"
            android:checked="true"
            app:thumbTint="#FFFFFF"
            app:trackTint="#4CAF50" />


        <ProgressBar
            android:id="@+id/progressLoading"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:indeterminate="true" />


        <ProgressBar
            android:id="@+id/progressDownload"
            style="?android:attr/progressBarStyleHorizontal"
            android:layout_width="200dp"
            android:layout_height="wrap_content"
            android:max="100"
            android:progress="40"
            android:progressTint="#4CAF50" />

        <androidx.recyclerview.widget.RecyclerView
            android:id="@+id/recyclerView"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:scrollbars="vertical"
            android:padding="8dp" />

        <Spinner
            android:id="@+id/spinnerCountry"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:entries="@array/country_list"
            android:spinnerMode="dropdown"
            android:prompt="@string/select_country"
            android:padding="8dp" />

        <ListView
            android:id="@+id/listNames"
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:dividerHeight="1dp"
            android:padding="8dp" />

        <AutoCompleteTextView
            android:id="@+id/autoCountry"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:hint="@string/enter_country"
            android:autofillHints="postalAddressCountry"
            android:completionThreshold="1"
            android:padding="8dp"
            android:textSize="16sp" />

    </LinearLayout>
</androidx.constraintlayout.widget.ConstraintLayout>
