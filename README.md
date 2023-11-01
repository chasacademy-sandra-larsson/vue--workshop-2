
# Vue #2: Vue komponenter, props, emits och slots
👋 Det har ännu inte varit någon föreläsning om detta, tror man kan klara sig på docs. Annars kommer en nästa vecka!  ✅ 

**Syftet med denna workshop:** 

* Setup av Vue-projekt med create vue
* Öva på komponenter och props i Vue
* Hur man kommunicerar uppåt (till parent) med $emit i child-komponenten och registrerar händelsen i parent-komponenten
* Vad slots är i Vue och vad man kan använda det till 

Använd dig av orginaldokumentationen [https://vuejs.org/](https://vuejs.org/). Du hittar även bra pedagogiskt material på Vue Mastery [https://www.vuemastery.com/](https://www.vuemastery.com/)

Bra lathund från Vue Mastery [https://www.vuemastery.com/vue-cheat-sheet/](https://www.vuemastery.com/vue-cheat-sheet/)

# Setup av Vue projekt

Nu använder vi oss av build-tools :-) Vi kommer använda oss av  [create vue](https://github.com/vuejs/create-vue) som bygger på Vite. Det finns även Vue CLI som bygger på Webpack (så att man vet skillnaden)

```
npm create vue@latest

```

Du får ett antal val, de flesta är givna. Ett tips är att du redan nu väljer Typescript ifall du vill bygga på med det senare (eller redan nu?). För att skriva js och inte i typescript tar du bort ```lang="ts"``` för komponenten samt lägger till ```"allowJS"=true``` i ```tsconfig.app.json```. 

Ta sedan bort onödig boilercode!


# 👩🏽‍💻 Övning 1: Rendera ut en lista av Cards

Här använder du dig av komponenter, props och $emits:
[https://vuejs.org/guide/components/registration.html
](https://vuejs.org/guide/components/events.html)
[https://vuejs.org/guide/components/props.html
](https://vuejs.org/guide/components/events.html)
[https://vuejs.org/guide/components/events.html
](https://vuejs.org/guide/components/events.html)

Du väljer själv temat för dina cards. Persondata, filmer, skräckkaraktärer 👻 -  whatever.

Du ska jobba med två komponenter:

**Card.vue** är ansvarig för att ta emot props som motsvarar den informaten som ska renderas ut på ditt valda Card. 

Kortet ska även ha en button som vid klick kommunicerar händelsen till parentkomponenten (App.vue) samt lämplig information om det kort som klickas - d.v.s använda $emit.

**App.vue** är ansvarig för att hålla en lista med objektdata för ditt tema, samt rendera ut alla Card med vardera information. Här ska du även ha en metod som tar emot en $emit och loggar till konsolen vilket kort som har klickats.

Styla efter egna preferenser!

# 👩🏽‍💻 Övning 2: Använda slots

Du fortsätter med koden från Övning 1.

Läs på vad slot är i Vue (väldigt likt children i React)
[https://vuejs.org/guide/components/slots.html](https://vuejs.org/guide/components/slots.html)

1. Använd en slot för att knappen för kortet ska passa användarprofilen. Exempelvis "Contact Dracula", "Watch The Shining"

2. Använd slots för att göra en s.k baslayout. I din baslayout ska det finns en header och footer - här väljer du innehåll själv. I en main ska du rendera ut listan av korten.

Voila! Lek sedan mad layouten hur du vill :-) 




# ✅ Redovisning:
* Du redovisar minst uppgiften för övningen. 
* ***Om du inte kan delta på workshopen, redovisar du ovanstående nästkommande workshop***







