# LinearLayout
```
<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical">
        //orientiation의 vertical 속성의 layout_weight속성 알아보기(주의사항은 layout_with속성을 0dp로)
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="200dp"
            android:layout_weight="1"
            android:orientation="horizontal">

            <TextView
                android:id="@+id/textView4"
                android:layout_width="0dp"
                android:layout_height="200dp"
                android:layout_weight="1"
                android:background="@color/colorAccent"
                android:text="One" />

            <TextView
                android:id="@+id/textView2"
                android:layout_width="0dp"
                android:layout_height="200dp"
                android:layout_weight="1"
                android:background="@color/colorPrimary"
                android:text="Two" />

            <TextView
                android:id="@+id/textView"
                android:layout_width="0dp"
                android:layout_height="200dp"
                android:layout_weight="1"
                android:background="@android:color/holo_blue_bright"
                android:text="Three" />
        </LinearLayout>
        
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="200dp"
            android:layout_marginTop="50dp"
            android:layout_weight="1"
            android:orientation="vertical">
            
            <TextView
                android:id="@+id/four"
                android:layout_width="match_parent"
                android:layout_height="0dp"
                android:layout_weight="1"
                android:background="@color/colorPrimary"
                android:text="four" />

            <TextView
                android:id="@+id/five"
                android:layout_width="match_parent"
                android:layout_height="0dp"
                android:layout_weight="3"
                android:background="@android:color/darker_gray"
                android:text="five" />

            <TextView
                android:id="@+id/six"
                android:layout_width="match_parent"
                android:layout_height="0dp"
                android:layout_weight="2"
                android:background="@android:color/background_dark"
                android:text="six" />
        </LinearLayout>

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="200dp"
            android:layout_marginTop="50dp"
            android:layout_weight="1"
            android:background="@android:color/darker_gray"
            android:orientation="vertical">

            <TextView
                android:id="@+id/textView8"
                android:layout_width="match_parent"
                android:layout_height="0dp"
                android:layout_weight="1"
                android:text="전화번호" />
            //view로 검은색의 밑줄 글여주기
            <view
                android:layout_width="match_parent"
                android:layout_height="1px"
                android:background="@android:color/background_dark" />

            <EditText
                android:id="@+id/editText"
                android:layout_width="match_parent"
                android:layout_height="0dp"
                android:layout_weight="2"
                android:ems="10"
                android:inputType="textPersonName" />

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="0dp"
                android:layout_weight="2"
                android:gravity="right"
                android:orientation="horizontal">
               //gravity로 버튼을 오른쪽에 보이기

                <Button
                    android:id="@+id/button2"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Button" />

                <Button
                    android:id="@+id/button"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="Button" />
            </LinearLayout>
        </LinearLayout>

    </LinearLayout>
</ScrollView>
