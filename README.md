# Noor Génération — site web

Site de l'ONG Noor Génération (Abidjan, Côte d'Ivoire), en ligne sur https://noorgeneration.org via GitHub Pages.

## Ajouter des photos / vidéos dans « Nos actions »

1. **Photos** : `Add file › Upload files`, glisse tes images et écris le chemin `media/` devant le nom
   (ex. `media/2026-12-yopougon-fournitures.jpg`). Garde chaque photo sous ~500 Ko (redimensionne à 1600 px de large).
2. **Vidéos** : mets-les sur YouTube (en « Non répertoriée » ou publique) et garde l'ID (la partie après `v=`).
   Les petits clips (< 25 Mo) peuvent aller dans `media/` en `.mp4`.
3. Ouvre `index.html`, cherche `const actions = [];` et ajoute une ligne par action :

```js
const actions = [
  { type:'photo',   src:'media/2026-12-yopougon-fournitures.jpg', titre:'Distribution de fournitures', date:'Déc. 2026', lieu:'Yopougon', cat:'Éducation' },
  { type:'youtube', id:'ID_YOUTUBE', titre:'Journée santé', date:'Janv. 2027', lieu:'Abobo', cat:'Santé & nutrition' },
];
```

4. `Commit changes` — le site se met à jour en 1 à 2 minutes.

⚠️ Avant de publier une photo d'enfant : accord écrit des parents/tuteurs, pas de nom complet, pas d'école ni d'adresse identifiable.
