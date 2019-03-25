# second
Android布局
## 利用线性布局实现以下界面
![](https://github.com/1061823154/second/blob/master/photo/QQ%E6%88%AA%E5%9B%BE20190325204340.png)

### 核心代码
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    >

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="20dp"
        android:orientation="horizontal">

        <TextView
            android:id="@+id/textView12"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="one,One" />

        <TextView
            android:id="@+id/textView13"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="one,Two" />

        <TextView
            android:id="@+id/textView11"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="one,Three" />

        <TextView
            android:id="@+id/textView14"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="one,Four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="20dp"
        android:orientation="horizontal"
        >

        <TextView
            android:id="@+id/textView22"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="two,One" />

        <TextView
            android:id="@+id/textView23"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="two,Two" />

        <TextView
            android:id="@+id/textView21"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="two,Three" />

        <TextView
            android:id="@+id/textView24"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="two,Four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="20dp"
        android:orientation="horizontal"
        >

        <TextView
            android:id="@+id/textView32"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="three,One" />

        <TextView
            android:id="@+id/textView33"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="three,Two" />

        <TextView
            android:id="@+id/textView31"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="TextView" />

        <TextView
            android:id="@+id/textView34"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="three,Four" />
    </LinearLayout>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="20dp"
        android:orientation="horizontal"
        >

        <TextView
            android:id="@+id/textView42"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="four,One" />

        <TextView
            android:id="@+id/textView43"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="four,Two" />

        <TextView
            android:id="@+id/textView41"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="four,Three" />

        <TextView
            android:id="@+id/textView44"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:text="four,Four" />
    </LinearLayout>
</LinearLayout>
```
### 运行截图：
![](https://github.com/1061823154/second/blob/master/photo/Screenshot_1553516971.png)

## 利用ConstrainLayout实现以下界面
![](https://github.com/1061823154/second/blob/master/photo/68747470733a2f2f696d672d626c6f672e6373646e696d672e636e2f32303139303331363233333035383534332e706e673f782d6f73732d70726f636573733d696d6167652f77617465726d61726b2c747970655f5a6d46755a33706f5a57356e6147567064476b2c736861.png)

### 核心代码：
```
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    >
    <Button
        android:id="@+id/B1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="RED"
        android:background="#DC143C"

        tools:ignore="MissingConstraints" />
    <Button
        android:id="@+id/B2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Orange"
        android:background="#FFA500"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        tools:ignore="MissingConstraints" />
    <Button
        android:id="@+id/B3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Yellow"
        android:background="#FFFF00"

        app:layout_constraintRight_toRightOf="parent"
        tools:ignore="MissingConstraints" />

    <Button
        android:id="@+id/B4"
        android:layout_width="60dp"
        android:layout_height="wrap_content"
        app:layout_constraintTop_toBottomOf="@id/B2"
        app:layout_constraintBottom_toTopOf="@+id/B7"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        android:text="Blue"
        android:textColor="#FFFFFF"
        android:background="#0000FF"
        />

    <Button
        android:id="@+id/B5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#008000"
        android:text="GREEN"
        app:layout_constraintRight_toLeftOf="@+id/B4"
        app:layout_constraintBaseline_toBaselineOf="@+id/B4"
        android:layout_margin="10dp"/>
    <Button
        android:id="@+id/B6"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="#4B0082"
        android:text="Indigo"
        android:textColor="#FFFFFF"
        app:layout_constraintLeft_toRightOf="@+id/B4"
        app:layout_constraintBaseline_toBaselineOf="@+id/B4"
        android:layout_margin="10dp"/>
    <Button
        android:id="@+id/B7"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:background="#EE82EE"
        android:text="Violet"
        app:layout_constraintBottom_toBottomOf="parent"
        />
</android.support.constraint.ConstraintLayout>
```
### 运行截图：
![](https://github.com/1061823154/second/blob/master/photo/Screenshot_1553517044.png)

## 利用表格布局实现如下界面：
![https://github.com/1061823154/second/blob/master/photo/68747470733a2f2f696d672d626c6f672e6373646e696d672e636e2f323031393033313632333432333535352e706e673f782d6f73732d70726f636573733d696d6167652f77617465726d61726b2c747970655f5a6d46755a33706f5a57356e6147567064476b2c73686164.png](https://github.com/1061823154/second/blob/master/photo/68747470733a2f2f696d672d626c6f672e6373646e696d672e636e2f323031393033313632333432333535352e706e673f782d6f73732d70726f636573733d696d6167652f77617465726d61726b2c747970655f5a6d46755a33706f5a57356e6147567064476b2c73686164.png)

### 核心代码
```
<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:stretchColumns="*">
<TableRow>
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="left"
        android:text="Open...."
        />
    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_gravity="right"
        android:text="Ctrl-O"
        />
</TableRow>
    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Open...."
            />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="right"
            android:text="Ctrl-S"/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Save As...."
            />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="right"
            android:text="Ctrl-Shift-S"/>
    </TableRow>
    <TableRow>
        <TextView
        android:layout_width="match_parent"
        android:layout_height="3dp"
        android:background="#050505"
        />
        <TextView
            android:layout_width="match_parent"
            android:layout_height="3dp"
            android:background="#050505"
            />
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Import...."
            />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="right"
            android:text=" "/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Export...."
            />
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="right"
            android:text="Ctrl-E"/>
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="match_parent"
            android:layout_height="3dp"
            android:background="#050505"
            />
        <TextView
            android:layout_width="match_parent"
            android:layout_height="3dp"
            android:background="#050505"
            />
    </TableRow>
    <TableRow>
        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_gravity="left"
            android:text="Quit"
            />
    </TableRow>
</TableLayout>
```
### 运行截图：
![](https://github.com/1061823154/second/blob/master/photo/Screenshot_1553517121.png)


