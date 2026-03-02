Cuarto archivo el cual son las listas iterables usando set, el codigo es el siguiente 
```dart
void main(){
  final numbers = [1, 2, 3, 4, 5, 6, 7 ,8, 9, 10];
  
  print ('lista original $numbers');
  
  print('Longitud : ${numbers.length}'); //el atributo length nos permite saber la longitud de una lista
  
  print('Indice 0: ${numbers[0]}'); //Para obtener o buscar un valor en especifico
  
  print('Primero: ${numbers.first}'); //Para obtener el primer valor de la lista
  
  print('Ultimo: ${numbers.last}'); //Para obtener el ultimo valor de la lista
  
  print('Inversa: ${numbers.reversed}'); //Para obtener el valores invertidos de la lista el hecho de aparecer en parentiesis se le llama Iterable (iterable en español), siendo listas, mapas o set los que pueden iterarse
  
  //Para convertir a lista 
  final numerosInvertidos = numbers.reversed;
  
  print('Iterable: ${numerosInvertidos}');
  
  print('Lista: ${numerosInvertidos.toList()}'); //Convertir de iterable a lista
  
  print('Lista: ${numerosInvertidos.toSet()}'); //Convertir de iterable a set la diferencia de mapas es que solo tiene valores, y en listas vs set, es que set no puede tener duplicados
  
  final numerosMayora5 = numbers.where((int number){
    return number > 5;
  });
  
  print('> 5: ${numerosMayora5.toSet()}'); //Busqueda, le ponemos .toSet para eliminar valores repetidos
  
  
}
```
como podemos ver, este codigo nos permite manipular listas, es decir, acceder a sus elementos, invertirlas, convertirlas a otros tipos de colección y filtrarlas usando condiciones.
