# Velora

Nasazení na běžný PHP hosting:

1. Nahraj celý obsah této složky do webového rootu (typicky `public_html`).
2. Hosting musí mít PHP 8+ se zapnutým rozšířením PDO SQLite a povolený zápis do této složky (pro `velora.sqlite` a `uploads/`).
3. Apache musí mít zapnuté `mod_rewrite`; soubor `.htaccess` zajišťuje adresy profilů ve tvaru `/username`.
4. V `api.php` odkomentuj a nastav odeslání mailu přes poskytovatele hostingu / SMTP. V implementaci je bezpečný ověřovací token; lokální demo zobrazí tlačítko pro dokončení ověření bez pošty.

Systém obsahuje registraci s hashovaným heslem, stav ověření e-mailu, volbu unikátní adresy, relace, nahrávání obrázků s validací typu i velikosti, editor profilových panelů a počítadlo návštěv.
