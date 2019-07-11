# Ud2_Ejemplo5
_Ejemplo 5 de la Unidad 2._ 

Vemos un ejemplo del ViewGroup LinearLayout al que le añadimos un EditText y un botón. Modificando el valor del atributo _orientation_ 
(_vertical_ u _horizontal_) podemos ver cómo los elementos se alinean en una orientación u otra.

Sólo hemos de fijarnos en el fichero _activity_main.xml_:

```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <EditText
        android:id="@+id/nombre"
        android:layout_width="220dp"
        android:layout_height="wrap_content"
        android:hint="@string/nombre" />

    <Button
        android:id="@+id/boton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="@string/enviar"/>

</LinearLayout>
```

Los textos del _EditText_ y del _Button_ se han insertado en el fichero _values/strings.xml_ y accedemos a él usando el símbolo @:

```
<resources>
    <string name="app_name">Ud2_Ejemplo5</string>
    <string name="nombre">Nombre</string>
    <string name="enviar">Enviar</string>
</resources>
```
Además se les ha asignado un _id_ a cada uno. Observad los símbolos @+.
