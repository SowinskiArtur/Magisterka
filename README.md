1. Opis problemu
    * Praca dotyczyć będzie utworzenia modelu mającego na celu klasyfikacje ofert produktowych na platformie e-commerce. Na platformie z której biorę dane rózni klienci
dodają różne produkty, często z własnymi drzewami kategorii, które jednak trzeba ujednolicić. Moja praca ma na celu zautomatyzowanie tego procesu, tak aby produkty
były kategoryzowane od razu po ich dodaniu, a praca ludzi została ograniczona do sprawdzania poprawności działania modelu.
2. Dlaczego problem jest ważny?
    * Zautomatyzowanie tego procesu może pozwolić na ograniczenie kosztów pracy, a nawet zwiększenie efektywności klasyfikacji.
3. Hipotezy badawcze
    * Lepsze wyniki będzie przyjmował model uczony na danych przetłumaczonych niż polskich.
    * Zastosowanie transformerów znacząco zwiększy skuteczność modelu.
4. Metody badawcze, zastosowane dane
    * Metody: tf-idf, transformers, pretrained models
    * Dane: dane będą pochodziły z bazy firmy (do ustalenia czy mogę pokazać dane produkcyjne, czy będę musiał użyć danych testowych/wygenerować dane)
5. Układ pracy
    1. Wstęp
        * opis jaką wartość biznesową może wprowadzić lepsze skategoryzowanie oferty produktowej na platformie e-commerce
    2. Data processing
        * przedstawienie zbioru danych
        * one hot encoding atrybutów produktów, na przykład czy produkt może mieć atrybut napięcie, moc itd.
        * preprocessing opisu produktu - unormowanie słów (lematyzacja, użycie małych liter), usunięcie najczęsciej wystepujących slów oraz znaków niealfanumerycznych
    3. Przeglad literatury oraz definicje pojęć związanych z NLP
        * tfidf
        * użycie modeli deep learningowych z zastosowaniem transformerów (pojęcie transformerów, encoderów, decoderów, atencji)
        * zastosowanie wstępnie wytrenowanych modeli, takich jak BERT/GPT/T5
    4. Modelowanie i opis/wizualizacja wyników
        * podejście do modelowania opisu oferty (tfitd, tranformery)
        * porównanie skuteczności na polskich opisach oraz opisach tłumaczonych automatycznie na angielski przez api google (lepsze wsparcie modeli dla języka  
          angielskiego)
        * model laczacy wyniki dla sieci nauczonej na opisach produktów oraz pozostalych parametrów (wprowadzenie kolejnej warstwy sieci neuronowej lub zbudowanie
          xgboosta na wyniku modelu oraz atrybutach)
        * podejście do ofert które nie będą pasować do żadnej kategorii (na przykład jakiś threshold który musi przewyższyć najwyższa wartość przyporządkowana do   
          kategorii)
    5. Wnioski
        * Jak wyniki wpłynęły na proces kategoryzacji
        * Co można zrobić, aby go polepszyć

Pracę będę pisał w wordzie, kody będą pisane w jupyter notebookach.
