Comentarios del programa. 

 /**
	 * @author Elias Peria�ez
	 * El constructor crea una conexion a 
	  COMPONENTES DEL GRUPO GULAG MAGICO
	 Grupo Gulag magico
	 Elias Peria�ez
	 Victor Barrios 
	 Javier S�nchez
	 Sara Correas
	 
	 
	 
	 
	 
	   
Reconocimiento-NoComercial-CompartirIgual 4.0 Internacional (CC BY-NC-SA 4.0)
Este es un resumen legible por humanos de (y no un sustituto) de la licencia . Descargo de responsabilidad .
Eres libre de:
Compartir : copiar y redistribuir el material en cualquier medio o formato
Adaptar - remezclar, transformar y construir sobre el material
El licenciante no puede revocar estas libertades mientras siga los t�rminos de la licencia.
Bajo los siguientes t�rminos:
Atribuci�n : debe otorgar el cr�dito apropiado , proporcionar un enlace a la licencia e indicar si se realizaron cambios . Puede hacerlo de cualquier manera razonable, pero no de ninguna manera que sugiera que el licenciante lo respalda a usted o a su uso.

No comercial: no puede usar el material con fines comerciales .

ShareAlike : si remixa, transforma o construye sobre el material, debe distribuir sus contribuciones bajo la misma licencia que el original.

Sin restricciones adicionales : no puede aplicar t�rminos legales o medidas tecnol�gicas que restrinjan legalmente que otros hagan cualquier cosa que la licencia permita.
Avisos:
No tiene que cumplir con la licencia para elementos del material en el dominio p�blico o donde su uso est� permitido por una excepci�n o limitaci�n aplicable .
No se dan garant�as. La licencia puede no otorgarle todos los permisos necesarios para su uso previsto. Por ejemplo, otros derechos como la publicidad, la privacidad o los derechos morales pueden limitar la forma en que utiliza el material. 

cc logo   
Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)
This is a human-readable summary of (and not a substitute for) the license. Disclaimer.
You are free to:
Share � copy and redistribute the material in any medium or format
Adapt � remix, transform, and build upon the material
The licensor cannot revoke these freedoms as long as you follow the license terms.
Under the following terms:
Attribution � You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

NonCommercial � You may not use the material for commercial purposes.

ShareAlike � If you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original.

No additional restrictions � You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.
Notices:
You do not have to comply with the license for elements of the material in the public domain or where your use is permitted by an applicable exception or limitation.
No warranties are given. The license may not give you all of the permissions necessary for your intended use. For example, other rights such as publicity, privacy, or moral rights may limit how you use the material.

 */
	 
	 
1//	 
CONSTRUCTOR  Conexi�n// 
Te da la oportunidad de conectarte directamente con una base de datos. En caso de que no se conecte, tiene que dar  un error y saltar un syso indicando que los par�metros est�n mal metidos. 

Dispone de try y catch por si las moscas. 
............................................................................
   1.1// El segundo constructor es el encargado de realizar la conexi�n programa base de datos. 
..................................................................................	 
2//
public ResultSet Consulta(String query)

 Se encarga de poner la cuery en la base de datos para poner los resultados obtenidos.
 .....................................................................................
3//  public String Consulta(String query, Boolean procesar)

Es un m�todo que se comunica con "ResultSet Consulta", para mostrar el resultado de la
consulta. 
......................................................................................

4//  public String Consulta(String query, Boolean procesar, int columna)

Es un m�todo que se comunica con consulta. Pone el resultado de columnas.

.......................................................................................

5//  public String ProcesarRset(ResultSet rset)

Indica el n�mero de columnas que tiene la tabla.Para esto, se vale  de ResultSetMetaData y rset.getMetaData() que se encarga de inicializar el while.Este a su vez, arranca un for que parte desde 1, ya que contamos columnas y el m�nimo es 1.
..............................................................................
6//  public String ProcesarRset(ResultSet rset, int columnas)

Se encarga de procesar el resultado obtenido. Se comunica con ProcesarRset.Y mira qu� tipo de dato le est�n metiendo. 
..............................................................................

7//  public boolean insertarDatos(String tabla, String[] campos, byte[] values)

Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los campos para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n. 
.............................................................................

8//  public boolean insertarDatos(String tabla, String[] campos, int[] values)
Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.

.............................................................................

9//  public boolean insertarDatos(String tabla, String[] campos, String[] values)

Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.
............................................................................

10// public boolean insertarDatos(String tabla, String[] campos, short[] values)

Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.

...........................................................................

11// public boolean insertarDatos(String tabla, String[] campos, long[] values)

Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.
............................................................................

12//  public boolean insertarDatos(String tabla, String[] campos, float[] values)

Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.

............................................................................

13//  public boolean insertarDatos(String tabla, String[] campos, boolean[] values)

Se encarga de insertar los datos a trav�s del sql y para ello se vale de una primera parte que es donde introducimos los datos de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.

.............................................................................

14// public boolean editarDatos(String tabla, String[] campos, String[] values, String condicion)

El principio del c�digo  est� para descargar el dato que quieras seleccionar de la tabla.Cuando tenemos todos, arranca un for que recorre los valores para insertar. Luego con un syso mostramos por consola los datos  metidos con aterioridad. Se conecta con el m�todo de conexi�n.

.............................................................................

15//  public boolean borrarFila(String tabla, String condicion)

En este caso lo que aparece en el comienzo del programa, es para borrar siempre que se cumpla la condici�n que marcar�amos. Se comunica con el m�todo conexi�n.
.............................................................................

16//  public String procesarRset(ResultSet rset, int columna)

Saca la informaci�n de la columna.

.............................................................................
17//   public void kill()
	Mata el programa. 
	 
	 
	 
	 