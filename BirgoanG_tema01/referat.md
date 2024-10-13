OpenGl referat 

OpenGL (Open Graphics Library) este o interfață de programare a aplicațiilor (API) care funcționează pe mai multe limbaje și platforme, utilizată pentru randarea graficii vectoriale 2D și 3D. Acest API este folosit, de obicei, pentru a interacționa cu o unitate de procesare grafică (GPU), pentru a obține randare accelerată hardware. De-a lungul timpului, au fost create diverse biblioteci și tehnologii ce se bazează pe OpenGL, printre care WebGL, Vulkan și OpenGL ES.


Avantaje:
 
  1.OpenGL funcționează pe mai multe platforme, cum ar fi Windows, macOS, Linux și dispozitive mobile, ceea ce îl face perfect pentru aplicații cross-platform. Aceasta înseamnă că dezvoltatorii pot scrie un singur cod sursă care să ruleze pe diferite sisteme, fără a fi nevoie să creeze versiuni separate pentru fiecare.
  
  2.Un alt avantaj al OpenGL este capacitatea sa de a crea și manipula grafică 3D complexă și efecte vizuale deosebite. Oferind un set bogat de instrumente pentru redarea luminii, texturilor și a altor detalii, OpenGL permite dezvoltarea de imagini și animații realiste de înaltă calitate.



Dezavantaje:
Compatibilitatea reprezintă o problemă în OpenGL, deoarece funcțiile disponibile variază între versiunile diferite, iar unele caracteristici nu sunt suportate pe toate platformele. Din această cauză, dezvoltatorii trebuie să scrie cod specific pentru fiecare sistem, ceea ce face adaptarea aplicațiilor mai complicată și necesită mai mult timp pentru testare și optimizare.




-->Cum explicați modelul de automat cu stări finite al OpenGL și cum afectează acest lucru procesul de randare al scenei 3D de către biblioteca grafică/API?

În OpenGL, există o stare globală activă în orice moment, care include setări precum culorile curente, texturile utilizate sau transformările aplicate. Dezvoltatorul comunică cu OpenGL printr-o serie de comenzi (de exemplu, pentru a desena forme sau a efectua transformări), iar aceste comenzi modifică progresiv starea sistemului. Fiecare modificare a stării se realizează în pași distincți, conducând treptat la rezultatul final al scenei 3D care este redată.

Astfel, orice acțiune în OpenGL, fie că este vorba de desenarea unui obiect sau de aplicarea unei transformări, alterează această stare globală. Scena 3D finală este produsul acumulării tuturor acestor schimbări succesive, pornind de la starea inițială implicită stabilită atunci când sistemul este inițializat.

