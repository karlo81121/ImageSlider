# Image Slider

Za zadatak je bilo potrebno napraviti slider koji koristi priložene slike (assets). Korisniku je omogućena interakcija sa slider-om putem strelica. Korišteni su div elementi unutar koda, ali su slike dodane u listu elemenata unutar HTML dokumenta te u polja (upperSliderImages i lowerSliderImages) unutar JS dokumenta. Prilikom pomicanja slika korišteni su indeksi polja (currentUpperFocus i currentLowerFocus) a veličine polja se dohvaćaju pomoću funkcije length (jQuery). Unutar JS dokumenta postoje dvije funkcije (za lijevu i desnu strelicu). S obzirom da se slider mora pomicati za dužinu slike koja je sljedeća na redu, korištena je funkcija width() koja vraća širinu slike. Funkcijom animate() je ostvareno pomicanje slider-a u desnu ili lijevu stranu a funkcijama append() i prepend() se dodaju sike na kraj i početak slider-a. Isto tako korištene su hide(), fadeOut() i fadeIn() funkcije odnosno efekti kojima se postižu dodatne animacije. Prilikom animate() funkcije mijenja se property 'left' unutar css-a za širinu slike te se u callback funkciji ponovo mijenja za određeni broj piksela kako bi se slike pomicale uvijek od istog mjesta na stranici. Za sve animacije korišteno je 400 milisekundi, osim za setTimeout() funkciju koja pomoću varijable arrowsEnabled (bool) ne dozvoljava ponovan klik na strelicu 500 milisekundi nakon što je ona kliknuta prvi put (iz razloga što se bržim klikovima animacija ne izvrši kako bi trebala). Na strelice je dodan hover efekt gdje su korištene četiri slike strelica iz datoteke assets.
