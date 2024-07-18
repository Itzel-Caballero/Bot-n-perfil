
# Bot-n-perfil

El componente BotonPerfil es un panel personalizado de Java Swing que contiene un botón (btnCuenta) y un panel adicional (Panel1) con varias etiquetas para mostrar información del usuario. Al hacer clic en el botón, se alterna la visibilidad del panel que contiene la información.

## Descripción
Este componente visual es un botón de perfil de usuario; este componente de Java permite ser usado en aplicaciones Java Swing, pudiendo ser añadido fácilmente en JFrame, JDialog, JPanel.

En este componente se puede modificar la imagen, la institución si se requiere colocar, el nombre del usuario, sus apellidos y su ID, de igual manera el color del botón, el color del panel y también el color de las tipografías; todo esto, por medio de métodos que se encuentran dentro de la clase. 


## Algunas posibles aplicaciones

| Aplicación                      | Descripción                                                                                                                                         |
|---------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| Aplicaciones de Gestión Escolar | Para mostrar información del estudiante al hacer clic en el botón, como número de control, nombre, apellidos, y la institución a la que pertenece.   |
| Aplicaciones de Gestión de Personal | Para mostrar información de los empleados, como número de identificación, nombre, apellidos, y departamento.                                            |
| Sistemas de Membresía           | Para mostrar información de miembros de un club o suscriptores de un servicio, con su identificación y detalles personales.                          |
| Aplicaciones de Registro de Eventos | Para mostrar información de los participantes de un evento, como conferencias, talleres, o competiciones.                                             |

## Características

 ### Funcionalidad de Mostrar/Ocultar Panel:
  •	El botón btnCuenta está configurado para alternar la visibilidad del panel jPanel1 cuando se hace clic en él. Esto se logra mediante el método btnCuentaActionPerformed, que invierte 
  el valor de visibilidad del panel.
  
 ### Icono Personalizado:
  •	El botón tiene un icono personalizado, especificado en su inicialización mediante btnCuenta.setIcon(new javax.swing.ImageIcon("ruta_del_icono"));. Este icono se puede cambiar a 
  cualquier imagen que desees mostrar en el botón.

 ### Texto del Botón:
  •	El botón tiene el texto "Cuenta", que se puede personalizar o cambiar según las necesidades de la aplicación.
  
 ### Configuración de Colores:
  •	Puedes personalizar el color de fondo y el color del texto del botón mediante el método setButtonColor(Color background, Color foreground). Esto permite que el botón se integre     
  visualmente con el resto de la interfaz de usuario.
  
 ### Uso de Eventos:
  •	El botón está configurado para responder a eventos de acción mediante un ActionListener. En el método initComponents(), se añade un ActionListener al botón para definir la acción a 
  realizar cuando se hace clic.
  
 ### Diseño y Ubicación:
  •	El botón está colocado dentro de un JLayeredPane, lo que permite una mayor flexibilidad en el diseño y la gestión de la disposición de los componentes superpuestos.

## API
  
#### Constructor
Inicializa el componente Boton1, configurando los componentes internos y estableciendo la visibilidad inicial del panel jPanel1 como oculta.

    public BotonCuentaP() {
        initComponents();
        jPanel1.setVisible(false);
        }

#### setlblInstitucionText	
Establece el texto de la etiqueta lblInstitucion.
Parámetro: text - El texto a mostrar en la etiqueta de la institución.

    public void setlblInstitucionText(String text) {
        lblInstitucion.setText(text);
        }

#### setlblNumerodeControl
Establece el texto de la etiqueta lblNumerodeControl.
Parámetro: 
text - El texto a mostrar en la etiqueta del número de control.

    public void setlblNumerodeControl (String text){
        lblNumerodeControl.setText(text);
        }

#### setlblNombre
Establece el texto de la etiqueta lblNombre.
Parámetro: 
text - El texto a mostrar en la etiqueta del nombre.

    public void setlblNombre (String text){
        lblNombre.setText(text);
        }

#### setlblApellido1Text
Establece el texto de la etiqueta lblApellido1.
Parámetro:
text - El texto a mostrar en la etiqueta del primer apellido.

     public void setlblApellido1Text (String text){
        lblApellido1.setText(text); 
        }

#### setlblApellido2Text
Descripción: Establece el texto de la etiqueta lblApellido2.
Parámetro: 
text - El texto a mostrar en la etiqueta del segundo apellido.

     public void setlblApellido2Text (String text){
        lblApellido2.setText(text);
        }

#### setEtiquetasColor
Establece el color de primer plano de todas las etiquetas del panel jPanel1.
Parámetro: 
foreground - El color de primer plano a aplicar a las etiquetas.

     public void setEtiquetasColor (Color foreground){
         lblInstitucion.setForeground(foreground);
         EtID.setForeground(foreground);
         lblNumerodeControl.setForeground(foreground);
         EtNombre.setForeground(foreground);
         lblNombre.setForeground(foreground);
         EtApellidos.setForeground(foreground);
         lblApellido1.setForeground(foreground);
         lblApellido2.setForeground(foreground);   
        }

#### setImagen
Establece el icono de la etiqueta lblImagen.
Parámetro: 
imagen - El icono a mostrar en la etiqueta de la imagen.

    public void setImagen(Icon imagen) {
        lblImagen.setIcon(imagen);
        }

#### setPanelColor
Establece el color de fondo del panel jPanel1.
Parámetro: 
background - El color de fondo a aplicar al panel.

    public void setPanelColor (Color background){
       jPanel1.setBackground(background);
       }

#### setButtonColor
Establece los colores de fondo y de primer plano del botón btnCuenta.

Parámetros:
background - El color de fondo a aplicar al botón.
foreground - El color de primer plano (texto) a aplicar al botón.

     public void setButtonColor(Color background, Color foreground) {
        btnCuenta.setBackground(background);
        btnCuenta.setForeground(foreground); 
        }


![image](https://github.com/user-attachments/assets/8408a069-884d-4ad0-9304-1eed340d2e52)

