# Exercice revue de code

Cette page contient une revue de code du travail pratique 1.

## Revue de code

::: info
Code du composant FlowerTable
:::

**Output**

```js{4}
function deleteFlower(flower: Flower): void {
    flowers.value.splice(flowers.value.indexOf(flower), 1);
    console.log('Fleur à supprimer->', flower);
    displayDeletionConfirmation.value = true;
}
```
##

::: info
Code du composant DuplicateForm
:::

**Output**

```js{4}
const flowerCopy = {
        id: (flowers.value.length + 1).toString(),
        name: duplicatedFlower.value.name,
        price: Number(duplicatedFlower.value.price),
        description: duplicatedFlower.value.description,
        stock: Number(duplicatedFlower.value.stock)
    }
```