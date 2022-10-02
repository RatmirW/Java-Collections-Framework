# Java-Collections-Framework

<p> - <a href="https://github.com/RatmirW/Java-Collections-Framework/blob/main/ListExample.java">List</a></p>

=================================== класс ArrayList ===================================
<table>
  <tr>
    <td>позиция:</td>
    <td>добавление:</td>
    <td>получение:</td>
    <td>удаление:</td>
  </tr>
  <tr>
    <td>начало</td>
    <td>O(1)</td>
    <td>O(1)</td>
    <td>O(n)</td>
  </tr>
  <tr>
    <td>середина</td>
    <td>O(1)</td>
    <td>O(1)</td>
    <td>O(n/2)</td>
  </tr>
  <tr>
    <td>конец</td>
    <td>O(1)</td>
    <td>O(1)</td>
    <td>O(1)</td>
  </tr>
</table>

<h2>Описание:</h2>
<ul>
  <li>реализован в виде динамического массива</li>
  <li>иерархия: Iterable -> Collection -> List -> AbstractList -> ArrayList</li>
  <li>расширяет AbstractList <E></li>
  <li>реализует List <E>, RandomAccess , Cloneable , Serializable</li>
  <li>потоко-небезопасен</li>
  <li>для работы в многопоточном режиме стоит использовать обертку: List list = Collections.synchronizedList(new ArrayList(...));</li>
  <li>Операции size , isEmpty , get , set , iterator и listIterator выполняются за постоянное время</li>
  <li>выдает исключение ConcurrentModificationException, если происходит попытка изменения структуры через итератор после создания списка</li>
  <li>может содержать null-элементы</li>
</ul> 
