//MainActivity.java
    package com.example.appmy;
    import android.content.Intent;
    import androidx.appcompat.app.AppCompatActivity;
    import android.os.Bundle;
    import android.view.View;
    import android.widget.Button;
    public class MainActivity extends AppCompatActivity {
    private Button button7,v;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);
    button7 = (Button) findViewById(R.id.button7);
    button7.setOnClickListener(new View.OnClickListener()
    {
    @Override
    public void onClick(View v){
    Next();}});}
    public void Next()
    {
    Intent intent =new Intent(this,Appmy2.class);

    startActivity(intent);
    }
    }
//Appmy2.java
    package com.example.appmy;

    import androidx.appcompat.app.AppCompatActivity;

    import android.os.Bundle;

    public class Appmy2 extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_appmy2);
    }
    }
//backnext_button.xml
    <?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle">
    <solid android:color="#F9FAFA"/>
    <corners android:radius="1000000dp"/>

</shape>
//custom_button.xml
    <?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle">
<solid android:color="#009688"/>
<corners android:radius="1000000dp"/>

</shape>
//retail_button.xml
    <?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle">
<solid android:color="#85C2D6CB"/>
<corners android:radius="1000000dp"/>

</shape>
//sactivity_button.xml
    <?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle">
<solid android:color="#03A9F4"/>
<corners android:radius="10dp"/>

</shape>
//sactivityretail_button.xml
    <?xml version="1.0" encoding="utf-8"?>
<shape xmlns:android="http://schemas.android.com/apk/res/android" android:shape="rectangle">
<solid android:color="#C3F9FAFA"/>
<corners android:radius="10dp"/>

</shape>
//activity_main.xml
    <?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".MainActivity">

<TextView
    android:layout_width="476dp"
    android:layout_height="62dp"
    android:text="Choose Categories that represent \n              what you want to see"
    android:textSize="20dp"
    tools:context=".MainActivity"
    tools:layout_editor_absoluteX="52dp"
    tools:layout_editor_absoluteY="16dp" />

<Button
    android:id="@+id/button3"
    android:layout_width="134dp"
    android:layout_height="131dp"
    android:background="@drawable/custom_button"
    android:text="Food"
    tools:layout_editor_absoluteX="52dp"
    tools:layout_editor_absoluteY="106dp" />

<Button
    android:id="@+id/button"
    android:layout_width="105dp"
    android:layout_height="111dp"
    android:background="@drawable/retail_button"
    android:text="Retail"
    tools:layout_editor_absoluteX="233dp"
    tools:layout_editor_absoluteY="126dp" />

<Button
    android:id="@+id/button2"
    android:layout_width="123dp"
    android:layout_height="129dp"
    android:background="@drawable/retail_button"
    android:text="Travel"
    tools:layout_editor_absoluteX="21dp"
    tools:layout_editor_absoluteY="276dp" />

<Button
    android:id="@+id/button4"
    android:layout_width="127dp"
    android:layout_height="132dp"
    android:background="@drawable/custom_button"
    android:text="Sport"
    tools:layout_editor_absoluteX="186dp"
    tools:layout_editor_absoluteY="255dp" />

<Button
    android:id="@+id/button5"
    android:layout_width="137dp"
    android:layout_height="141dp"
    android:background="@drawable/retail_button"
    android:text="Entertainment"
    tools:layout_editor_absoluteX="233dp"
    tools:layout_editor_absoluteY="417dp" />

<Button
    android:id="@+id/button6"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:background="@drawable/backnext_button"
    android:text="Back"
    tools:layout_editor_absoluteX="31dp"
    tools:layout_editor_absoluteY="667dp" />

<Button
    android:id="@+id/button7"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:text="Next"
    android:background="@drawable/backnext_button"
    tools:layout_editor_absoluteX="307dp"
    tools:layout_editor_absoluteY="667dp" />

</androidx.constraintlayout.widget.ConstraintLayout>
//activity_appmy2.xml
    <?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto"
xmlns:tools="http://schemas.android.com/tools"
android:id="@+id/relativeLayout"
android:layout_width="match_parent"
android:layout_height="match_parent"
tools:context=".Appmy2">

<TextView
    android:id="@+id/textView"
    android:layout_width="648dp"
    android:layout_height="80dp"
    android:layout_marginStart="115dp"
    android:layout_marginTop="16dp"
    android:text="@string/dashboard"
    android:textSize="30sp"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    tools:context=".MainActivity" />

<Button
    android:id="@+id/button8"
    android:layout_width="104dp"
    android:layout_height="113dp"
    android:layout_marginStart="60dp"
    android:layout_marginTop="176dp"
    android:text="@string/food_n_8_offers"
    android:textSize="15sp"
    android:background="@drawable/sactivity_button"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent" />

<Button
    android:id="@+id/button9"
    android:layout_width="101dp"
    android:layout_height="110dp"
    android:layout_marginStart="38dp"
    android:layout_marginTop="32dp"

    android:layout_marginEnd="108dp"
    android:layout_marginBottom="24dp"
    android:background="@drawable/sactivityretail_button"
    android:text="@string/travel_n_0_offers"
    app:layout_constraintBottom_toTopOf="@+id/button11"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toEndOf="@+id/button8"
    app:layout_constraintTop_toBottomOf="@+id/textView3" />

<Button
    android:id="@+id/button10"
    android:layout_width="109dp"
    android:layout_height="114dp"
    android:layout_marginStart="67dp"
    android:layout_marginTop="19dp"
    android:layout_marginEnd="28dp"
    android:layout_marginBottom="7dp"
    android:background="@drawable/sactivityretail_button"
    android:text="@string/entertinment_n2_offers"
    app:layout_constraintBottom_toTopOf="@+id/button12"
    app:layout_constraintEnd_toStartOf="@+id/button11"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/button8" />

<Button
    android:id="@+id/button11"
    android:layout_width="107dp"
    android:layout_height="109dp"
    android:layout_marginStart="38dp"
    android:layout_marginTop="24dp"
    android:layout_marginEnd="107dp"
    android:background="@drawable/sactivity_button"
    android:text="@string/sport_n5_offers"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toEndOf="@+id/button10"
    app:layout_constraintTop_toBottomOf="@+id/button9" />

<Button
    android:id="@+id/button12"
    android:layout_width="104dp"
    android:layout_height="104dp"
    android:layout_marginStart="60dp"
    android:layout_marginTop="7dp"
    android:layout_marginEnd="50dp"
    android:background="@drawable/sactivityretail_button"
    android:text="@string/retail_n_0_offers"
    app:layout_constraintEnd_toStartOf="@+id/button13"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/button10" />

<Button
    android:id="@+id/button13"
    android:layout_width="102dp"
    android:layout_height="100dp"
    android:layout_marginStart="50dp"
    android:layout_marginTop="12dp"
    android:background="@drawable/sactivityretail_button"
    android:text="@string/add_wight"
    app:layout_constraintStart_toEndOf="@+id/button12"
    app:layout_constraintTop_toBottomOf="@+id/button11" />

<TextView
    android:id="@+id/textView2"
    android:layout_width="292dp"
    android:layout_height="89dp"
    android:layout_marginStart="120dp"
    android:layout_marginTop="12dp"
    android:text="@string/aravinnd_n_nayak"
    android:textSize="40sp"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/button12" />

<TextView
    android:id="@+id/textView3"
    android:layout_width="216dp"
    android:layout_height="59dp"
    android:layout_marginStart="90dp"
    android:layout_marginEnd="13dp"
    android:layout_marginBottom="21dp"
    android:text="@string/welcome"
    android:textSize="50sp"
    app:layout_constraintBottom_toTopOf="@+id/button8"
    app:layout_constraintEnd_toStartOf="@+id/textView"
    app:layout_constraintHorizontal_bias="0.0"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/textView" />


</androidx.constraintlayout.widget.ConstraintLayout>
//strings.xml
<resources>
<string name="app_name">Appmy</string>
<string name="dashboard">Dashboard</string>
<string name="welcome">Welcome</string>
<string name="Dashboard">Dashboard</string>
<string name="aravinnd_n_nayak">Aravinnd\n Nayak</string>
<string name="entertinment_n2_offers">Entertinment\n2 Offers</string>
<string name="travel_n_0_offers">Travel\n 0 Offers</string>
<string name="sport_n5_offers">Sport\n5 Offers</string>
<string name="retail_n_0_offers">Retail\n 0 Offers</string>
<string name="add_wight">add wight</string>
</resources>
