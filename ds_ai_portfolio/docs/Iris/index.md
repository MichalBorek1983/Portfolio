
#  Analiza Danych EDA Irysów: Eksploracja Domenowa

Czy można odróżnić gatunek kwiatu, patrząc jedynie na liczby? Ten projekt to fascynująca podróż przez dane, w której botanika łączy się z inżynierią danych.

Przeprowadziłem szczegółową Eksploracyjną Analizę Danych (EDA) irysów, aby wydobyć z tabel to, co niewidoczne na pierwszy rzut oka. Zapraszam do lektury, w której krok po kroku odkrywam wzorce rządzące naturą, prezentując trafne wnioski i obserwacje rzucające nowe światło na ten klasyczny zbiór danych.


<a href="iris.ipynb" class="md-button md-button--primary">Pobierz Notebook</a>

<iframe
    id="content"
    src="iris.html"
    width="100%"
    style="border:1px solid black;overflow:hidden;"
></iframe>
<script>
function resizeIframeToFitContent(iframe) {
    iframe.style.height = (iframe.contentWindow.document.documentElement.scrollHeight + 50) + "px";
    iframe.contentDocument.body.style["overflow"] = 'hidden';
}
window.addEventListener('load', function() {
    var iframe = document.getElementById('content');
    resizeIframeToFitContent(iframe);
});
window.addEventListener('resize', function() {
    var iframe = document.getElementById('content');
    resizeIframeToFitContent(iframe);
});
</script>
4