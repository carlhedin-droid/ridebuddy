# Busbuddy

Avgångstavla för bussarna mellan hållplatserna kring Sandudden/Träkvista (Ekerö) och Brommaplan. Kan delas med grannar – var och en väljer sina hållplatser.

- **Till Brommaplan:** en gemensam lista i tidsordning med avgångar från ens utresehållplatser, med etikett "från …". Bussar som har Brommaplan som slutstation eller går via Brommaplan (samma tur avgår senare därifrån) visas. En buss som stannar vid flera hållplatser visas vid den första i prioritetsordning. Med gångtid hemifrån per hållplats (inställning) visas "Gå HH:MM", "Gå nu", "Spring" eller "Hinner inte". Gångtiderna följer inte med i delningslänken.
- **Från jobbet:** under ⚙️ → Arbetsplats anger man namn/adress (t.ex. "PwC, Torsgatan 21"), stationen man åker från (t.ex. S:t Eriksplan) och gångtid dit. Fliken kopplar tunnelbanan (samma tur-id vid jobbstationen och vid Brommaplan) till bussarna hem och visar för varje buss det sista tåget man hinner byta från – alltså när man ska gå från jobbet för kortast väntan på Brommaplan, väntetiden och ankomsten till hemhållplatsen. Alternativ som är sämre på alla sätt (gå tidigare men inte komma fram tidigare eller närmare) visas inte. Jobbstationen följer inte med i delningslänken.
- **Hem från Brommaplan:** bussar som stannar vid någon av ens hemresehållplatser. Bussen visas med den första hållplatsen i prioritetsordning som den passerar, och ankomsttiden dit. Hållplatser markerade som reserv visas under "Reservalternativ". Vilka linjer som gäller räknas ut från SL:s realtidsdata (samma linje och tur-id vid Brommaplan och vid hållplatsen); restiderna lärs in för turer som ligger för långt fram.
- **Hinner gå / Spring / Hinner inte:** utgår från gångtiden från tunnelbanan till bussen på Brommaplan (inställning, förval 4 min; springa = halva tiden).
- **Skjuts:** tryck på Skjuts vid en avgång hem. WhatsApp öppnas med ett färdigt meddelande med linje, avgångstid och upphämtningstid vid hållplatsen man kliver av vid.
- **Inställningar (⚙️):** hållplatser för utresa och hemresa i prioritetsordning, reservhållplatser, gångtid, namn och WhatsApp-nummer. Allt sparas bara i telefonen.
- **Dela:** knappen i inställningarna skapar en länk (`?s=…`) med samma hållplatser och gångtid, men utan namn och nummer.
- **Självuppdatering:** sidan laddar om sig själv när en ny version har publicerats.

Förval: utresa Sanduddens vägskäl, Träkvista, Träkvista idrottsplats; hemresa samma tre plus Ekvägen som reserv. SL-id: Sandudden 3080, Sanduddens vägskäl 3081, Träkvista 3065, Träkvista idrottsplats 3069, Ekvägen 3047, Brommaplan 9109.

Data i realtid från SL:s öppna API (SL Transport, via Trafiklab). Ingen nyckel krävs.
Publiceras på https://busbuddy.pages.dev (Cloudflare Pages) från grenen `main`. Den gamla adressen carlhedin-droid.github.io/ridebuddy/ skickar vidare dit och tar med sparade inställningar.
