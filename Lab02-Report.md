# รายงานผลการทดลอง

<ศศิกร กอเสนาะรส> <รหัสนักศึกษา 603410063-8>

## Relative Layout

แสดง Control `title` และ `Detail`

```xml

```

แอดทริบิ้วที่แสดงความสัมพันธ์ระหว่าง control ทั้งสอง

```xml

```

## Linear Layout

แสดง Control `to`, `subject`, `tag` และ `message`

```xml

```

อธิบายความแตกต่างระหว่าง vertical และ horizontal orientation

vertical orientation คือการจัดเรียงให้อยู่ในแนวตั้ง ส่วน horizontal orientation คือการจัดเรียงให้อยู่ในแนวนอน

## Constrant Layout

จงออกแบบและสร้างหน้า Constrant layout สำหรับแสดงข้อมูลนักศึกษา ประกอบไปด้วย รูปโปรไฟล์ รูปพื้นหลัง ชื่อ-นามสกุล รหัสนักศึกษา และเกรดเฉลี่ยรวม

activity_constant.xml
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".ConstantActivity">


    <ImageView
        android:id="@+id/imageView6"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        app:srcCompat="@color/colorPrimaryDark" />

    <ImageView
        android:id="@+id/imageView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentStart="true"
        android:layout_alignParentTop="true"
        android:layout_alignParentEnd="true"
        android:layout_marginStart="0dp"
        android:layout_marginTop="-200dp"
        android:layout_marginEnd="0dp"
        app:srcCompat="@drawable/friends" />

    <de.hdodenhof.circleimageview.CircleImageView
        android:id="@+id/profile_image"
        android:layout_width="76dp"
        android:layout_height="204dp"
        android:layout_alignParentStart="true"

        android:layout_alignParentEnd="true"
        android:layout_marginStart="89dp"
        android:layout_marginTop="90dp"
        android:layout_marginEnd="96dp"
        android:src="@drawable/profile"
        app:civ_border_color="#FFFFFF"
        app:civ_border_width="2dp" />

    <LinearLayout
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical">

        <TextView
            android:id="@+id/textView"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"

            android:layout_marginStart="50dp"
            android:layout_marginTop="250dp"
            android:layout_marginEnd="10dp"
            android:layout_marginBottom="100dp"
            android:text="ศศิกร กอเสนาะรส"
            android:textColorHighlight="#9C27B0"
            android:textSize="20sp"
            android:textStyle="bold" />

        <TextView
            android:id="@+id/textView1"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"

            android:layout_marginStart="40dp"
            android:layout_marginTop="-100dp"
            android:layout_marginEnd="0dp"
            android:layout_marginBottom="50dp"
            android:text="รหัสนักศึกษา 603410063-8"
            android:textColorHighlight="#9C27B0"
            android:textSize="18sp" />

        <TextView
            android:id="@+id/textView2"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"

            android:layout_marginStart="40dp"
            android:layout_marginTop="-50dp"
            android:layout_marginEnd="0dp"
            android:layout_marginBottom="100dp"
            android:text="เกรดเฉลี่ยรวม : 3.33"
            android:textColorHighlight="#9C27B0"
            android:textSize="18sp" />

    </LinearLayout>

</RelativeLayout>
