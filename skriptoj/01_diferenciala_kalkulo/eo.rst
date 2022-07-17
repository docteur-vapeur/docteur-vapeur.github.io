Superrigardo de la diferenciala kalkulo
=======================================

La infinitezima kalkulo estas branĉo de matematiko, kiu studas la senhaltajn
ŝanĝojn. Oni povas disigi ĝin en du fakon :
- La  *diferenciala* kalkulo servas por kalkuli la derivaĵojn de funkcioj, tio
  estas la tujan variadon.
- La integrala kalkulo utilas por integrali funkciojn kaj determini la amasiĝon
  de valoroj.

Ĉi tiu video prezentas superrigardon de la diferenciala kalkulo.

Difinu la problemon : oni havas funkcion :math:`f(x)` kaj oni volas determini
ĝian ŝanĝon aw la krutecon de la deklivo de la grafeo. Funkcio, kiu rapide
pliiĝas, havas altan ŝanĝon dum konstanta funkcio havas nulan ŝanĝon ĉar la
valoro de :math:`f(x)` ne varias rilate al x.


Oni povas kalkuli la deklivon de funkcio elektante du punktojn kaj dividante la
ŝanĝon rilate al ipsilono-akso per la ŝanĝon rilate al x-akso.

.. math::
   \\frac{\\Delta y}{\\Delta x} = \\frac{f(a + \\Delta x) - f(a)}{Delta x}

Ekzemple, kun la funkcio :math:`f(x) = 1 + 2x`, oni elektas du punktojn - unu
signita :math:`a` kaj la alia estas movita per valoro :math:`\\Delta x`. Oni
aplikas la formulon por akiri deklivon de 2, kio signifas ke pliiĝi :math:`x`
per unu unuo pliiĝas la funkcio :math:`f(x)` per du unuoj. La kalkulo estas
facila en ĉi tiu ekzemplo ĉar la deklivo estas konstanta ĉie sur la funkcio,
sed la aferoj estas pli malfacila kun kun pli kompleksaj funkcioj.


Ekzemple, ni provu kalkuli la deklivon de la funkcio :math:`f(x) = x^2` ĉe la
punkto :math:`x = 1`. La deklivo reprezentas la rapidecon je kiu la funkcio
ŝanĝiĝas. Oni povas ilustri la deklivon kun tangeto - linio kiu tuŝas la kurbon
ĉe unu punkto. Por proksimumi la valoron de la deklivo, oni povas uzi la
antawan ekvacion.

.. math::
   \\frac{\\Delta y}{\\Delta x} = \\frac{f(a + \\Delta x) - f(a)}{Delta x}

Oni bezonas du punktojn. Ni elektu :math:`x = 1; f(x) = 1` por la unua kaj
:math:`x = 2; f(x) = 4` por la dua. La linio, kiun oni akiras per ĉi tiu
metodo, nomiĝas sekanto. Ni vidas, ke ĝi estas malbona proksimumado de la
tangeto. Por plibonigi la kalkulon de la deklivo, oni povas proksimigi la
duan punkton al la unua punkto. Ekzemple, elektante
:math:`x = 3/2; f(x) = 9/4`, oni akiri sekanton pli proksime de la dezirata
rezulto. Oni dawras tiel, elektanta pli kaj pli proksimajn punktojn por
plibonigi la kalkulon de la deklivo. Pli formale, ĉi tiu procezo estas
reprezentata per la ekvacio

.. math::
   f'(x) = lim_{\\Delta x \\to 0}\\frac{f(a + \\Delta x) - f(a)}{Delta x}.

Ĉi tiu simbolo, *la limeso kiam delto x alproksimiĝas al nulo*, signifas ke
oni kalkulas la valoro al kiu la funkcio konverĝas kiam delto x iĝas pli kaj
pli proksima al nulo. Ni vidos kiel kalkuli ĉi tiu ekvacion.

Parto I : la limesoj
--------------------

Limeso estas la kvanto al kiu funkcio alproksimiĝas kiam ĝia enigo
alproksimiĝas valoro.

Ekzemple, supozu ke oni volas determini la limeso de la funkcio
:math:`(x^3)/2 - x` kiam x alproksimiĝas al la valoro 2. Elektante valorojn de
x, kiu proksimiĝas al 2, oni taksas la funkcion f(x). La tabelo montras, ke la
funkcio konverĝas al la valoro du; oni diras ke la limeso egalas du.

Alia ekzemplo : oni serĉi la limeso de la funkcio :math:`(x^3 -1)/(x -1)` kiam
x alproksimiĝas al unu. La funkcio ne estas difinata ĉe la punkto :math:`x = 1`
ĉar se oni anstatawigi x per ĉi tiu valoro, oni akiras divido per nulo. Oni
povas tamen taksi la limeso : elektante punktojn, kiuj alproksimiĝas al
:math:`x = 1`, oni vidas, ke la funkcio alproksimiĝas al la valoro 3. Kvankam
la funkcio ne estas difinata ĉe tiu punkto, la limeso estas kalkulebla.

Ekzamenu alian kason kun la funkcio :math:`1/x`. Oni serĉas la limeso kiam x
alproksimiĝas al nulo. Sur la grafeo, oni vidas, ke la funkcio alproksimiĝas
al malsamaj valoroj law la flanko de la alproksimiĝo. Komencante de dekstre,
f(x) alproksimiĝo al pozitiva malfinio. Oni reprezentas ĉi tiu direkto
aldonante la simbolon "+" en la skribo de la limeso. Oni povas ankaw proksimiĝi
la valoro :math:`x = 0` komencante de la maldekstre, kio reprezentas kun la
simbolo "minus". La limeso de ĉi tiu flanko estas minus malfinio.

Ni revenu al kalkulo de la derivaĵo. Oni volas taksi la esprimon

.. math::
   f'(x) = lim_{\\Delta x \\to 0}\\frac{f(a + \\Delta x) - f(a)}{Delta x}

por akiri la tujan variadon de la funkcio. Post disvolvo kaj simpligo de la
funkcio, oni akiras

.. math:: .. limeso de du-a plus delto x kiam delto x alproksimiĝas al nulo
   f'(x) = lim_{\\Delta x \\to 0}\\2a + \\Delta x.

Ĉar delto x alproksimiĝas al nulo, ĝia valoro iĝas pli kaj pli neglektebla
rilate du. La limeso de ĉi tiu esprimo do egalas du, kiu kongruas kun la tuja
variado de la funkcio :math:`x^2` ĉe la punkto :math:`x = 1`.


Anstataw kalkuli la derivaĵo ĉe unu aparta punkto, oni povas uzi arbitran x
punkton. Reuze la sama procedo kaj uze x anstataw unu, oni akiras :


.. math::
   f'(x) = 2x

Parenteze, la simbolo f'(x), eltrovita per Euler kaj popularigita per Lagrange,
ne estas la sola simbolo por reprezenti derivon. Oni povas ankaw uzi la
notacion de Leibniz - d sur dx, aw la notacion de Newton, kiu konsistas en
aldoni punkton sur la dependa variablo.

Oni povas uzi la difinon de la derivo kaj la koncepton de limeso por kalkuli
la derivaĵon de aliaj funkcioj. Ekzemple, uze la saman esprimon, oni povas
kalkuli la derivaĵo de la funkcio :math:`1/x`. Ekzistas tamen aliaj teknikoj,
kiuj simpligas la kalkulon de derivaĵoj. Ni vidos kelkajn el ili.


Parto II : kalkaj reguloj de derivo
-----------------------------------

Ni komencu kun la derivaĵo de konstanta termino : aplikante la difinon de la
derivo, oni akiri nula valoro por ĉiuj valoroj.

Alia grava tekniko estas la regulo de la potencoj. Por funkcio :math:`x^n`, la
derivaĵo egalas la esprimo :math:`nx^(n-1)`. Oni povas uzi ĉi tiun regulon por
derivi funkcioj kun realaj eksponentoj, ĉu ili estas pozitivaj, negativaj aw
frakciaj.

La derivo estas lineara operacio, tio estas ĝi verigi la sekvan ekvacion :


.. math::
   d/dx ah + bg = ah' + bg'

Oni deduktas la regulon de la multiplikaĵo kun un skalaro, la regulon de la
sumo kaj la regulon de la diferenco.

La regulo de la produto diras, ke la derivaĵo de la produto de du funkcioj *f*
kaj *g* egalas

.. math::
   f'g + fg'

Oni povas kombini la regulon de la produto kun, ekzemple, la regulon de la
potencoj por kalkuli la derivaĵo de funkcio farita de produto.

La ĉena regulo permesas al oni taksi la derivaĵon de komponitaj funkcioj. Ĉi
tiuj funkcioj okazas, kiam la rezulto de funkcio estas uzata kiel argumento de
alia funkcio. Ekzemple, se :math:`f(x) = x^2` kaj :math:`g(x) = x - 1`, tiam


.. math:: .. f komponita kun g
   f \\circle g = f(g(x)) = {(x - 1)}^2

La ĉena regulo estas donita per la sekva ekvacio :

.. math::
   f(g(x))' = f'(g(x)) g'(x)

Kun la antawa ekzemplo, oni do kalkulas :

.. math::
   \\frac{d}{dx} {(x - 1)}^2 = 2{(x - 1)}^{2 -1} \\frac{d}{dx} x = 2(x - 1)

Ekzistas multaj aliaj reguloj por derivi funkcioj, ekzemple, trigonometriaj,
eksponentaj aw logaritma, kiuj estas prezentataj en pli kompletaj rimedoj.


Parto III : maksimumoj kaj minimumoj
------------------------------------

La diferenciala kalkulo povas servi por determini la lokoj de maksimumoj kaj
minimumoj - la ekstremumoj - de funkcio, tio estas la valoroj de f(x), kiuj
estas pli alta aw pli malalta ol la valoroj ĉirkaŭe. Ni rimarkas, ke se la
deklivo estas pozitiva, oni povas dekstre determini valoron de x, kiu kondukas
al valoro de f(x) pli alta. Se la deklivo estas negativa, oni povas maldekstre
trovi valoron, kiu kondukas al valoro de f(x) pli alta. Tial, la ekstremumoj
nepre troviĝas sur punktoj sur kiuj la derivaĵo de la funkcio estas nula. Por
determini la ekstremumoj de funkcio, oni devas derivi ĝin kaj trovi ĝiajn
nulejojn.

Ekzemple, reprenante la funkcion :math:`f(x) = (x^3)/2 - x`, oni aplikas la
regulon de la potencoj por kalkuli ĝia derivaĵo : :math:`f'(x) = 3/2 x^2 - 1`.
Solve ĝin por trovi ĝian nulejojn, oni povas determini la lokoj de la
ekstremumoj.

Parto IV : kelkaj aplikaĵoj de diferenciala kalkulo
---------------------------------------------------

La derivaĵo estas uzataj en multaj fakoj; ĉi tiu sekcio prezentas kelkaj
simplajn aplikaĵojn.

Oni povas uzi la derivo por kalkuli la rapidon de objekto law ĝia pozicio.
Ni diru, ke la funkcio :math:`x(t)` priskribas la pozicion en metroj de objekto
rilate la tempo *t* en sekundoj. La rapido kongruas kun la tuja variado de la
pozicio; oni povas do akiri ĝin derive la pozicion kaj generi la funkcion
:math:`x'(t)`, en metroj je sekundoj. La akcelo priskribas kiel la rapido
ŝanĝas; oni povas do akiri ĝin derive la rapidon kaj generi la funkcion
:math:`x''(t)`, en metroj je sekundoj je sekundoj. La funkcioj de rapido kaj
akcelo permesas poste akiri utilajn informojn por kompreni la trajektorion de
la objekto, ekzemple, la momentoj en kiuj la objekto estas senmova aw la
periodoj en kiuj la akcelo estas pli intensa.


La derivaĵoj permesas aw kompreni la elektrajn cirkvitojn. Kondensilo,
ekzemple, estas simplaj komponantoj, kiu povas enmagazenigi elektrajn ŝarĝojn.
La elektra kurento *i*, kiu transiras la kondensilon rilate tempo estas ligata
al la kapacitanco *C* specifa al la komponanto kaj al la derivaĵo de la elektra
potencialo.

.. math::
   i(t) = C \\frac{dv(t)}{dt}

La derivo do permesas kompreni la elektrajn kurentojn en la cirkvitoj.


La diferenciala kalkulo estas ligata al la integrala kalkulo. La integralo
estas fakte la reverso operacio de la derivo. Ĝi permesas kalkuli amasiĝon de
valoroj por akiri, ekzemple, la ekzaktan areon de malregulaj surfacoj aw la
pozicion de objekto rilate al ĝia rapido.


Mallonge,
- la diferenciala kalkulo estas fako de infinitezima kalkulo que servas por
  determini la tuja variado de funkcion.
- Kun la limesoj, oni povas difini la derivon.
- Ekzistas reguloj, kiuj permesas derivi funkciojn pli facile sen uze la
  limesojn.
- Laste, la diferenciala kalkulo estas uzata en problemoj, en kiuj oni volas
  trovi la rapido de ŝanĝo de valoroj.
