Third exercise in second week on eduweb.pl bootcamp.
======

Created html file with stuff from exercise 3 in week 2.

Exercise 3:
Ajaxowy polyfill dla funkcji fetch

Napisz polyfill dla funkcji fetch (nie będziemy się tutaj trzymać dokładnie tego, w jaki sposób ona działa, stworzysz jedynie prostą jej wersję). Wykorzystaj obiekt XMLHttpRequest w ten sposób, aby docelowo korzystanie z funkcji fetch wyglądało następująco:
fetch("url", function(data) {
		console.log("Sukces");
		console.log(data);
	}, 
	function(err) {
		console.log("Wystąpił błąd!");
		console.log(err);
	});
a zatem jako pierwszy argument przekazujemy adres URL (wyślij pod niego zapytanie GET), jako drugi funkcję, którą należy wykonać jeśli wszystko się powiedzie (przekaż jej
pobrane dane), a jako trzeci funkcję, która wykona się na wypadek błędu (przekaż jej obiekt z błędem lub komunikat tekstowy). W nowoczesnych przeglądarkach istnieje już
funkcja fetch, a zatem aby jej nie nadpisywać, możesz nadać jej inną nazwę. Jako adres URL, z którego pobierane bedą dane, możesz wykorzytać https:// jsonplaceholder.typicode.com/users