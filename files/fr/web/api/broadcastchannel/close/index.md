---
title: BroadcastChannel.close()
slug: Web/API/BroadcastChannel/close
page-type: web-api-instance-method
translation_of: Web/API/BroadcastChannel/close
browser-compat: api.BroadcastChannel.close
---
{{APIRef("BroadCastChannel API")}}

La méthode **`BroadcastChannel.close()`** ferme la connexion au canal sous-jacent, permettant à l'objet d'être libéré par le ramasse-miettes. Cette tâche est obligatoire puisqu'il n'y a aucun autre moyen pour le navigateur de savoir si ce canal est encore nécessaire.

{{AvailableInWorkers}}

## Syntaxe

```js
canal.close();
```

## Exemple

```js
// Connexion au canal
const bc = new BroadcastChannel('canal_test');

// Autres opérations (tel que postMessage, …)

// Lorsque les traitements sont terminés, déconnexion du canal
bc.close();
```

## Spécifications

{{Specifications}}

## Compatibilité des navigateurs

{{Compat}}

## Voir aussi

- [`BroadcastChannel`](/fr/docs/Web/API/BroadcastChannel), l'interface à laquelle elle se rapporte.