
#  Analiza Danych EDA Titanic: Eksploracja Domenowa

Zapraszam do zapoznania się z projektem, który przenosi nas na pokład "niezatapialnego" statku – tym razem jednak patrzymy na niego przez pryzmat danych.

Celem tej analizy było odkrycie ukrytych wzorców w chaosie ewakuacji. Czy zasada "kobiety i dzieci najpierw" była faktycznie przestrzegana? Jaką rolę odgrywał status majątkowy? W tym projekcie znajdziesz mnóstwo trafnych wniosków i obserwacji, które rzucają nowe, analityczne światło na losy pasażerów Titanica. Przygotuj się na podróż przez dane, która pokazuje potęgę analizy eksploracyjnej.

<a href="Titanic.ipynb" class="md-button md-button--primary">Pobierz Notebook</a>

<iframe
    id="content"
    src="Titanic.html"
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