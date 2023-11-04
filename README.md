# My first repository

# My name is Yehor

![my image](https://github.com/YehorSlivinskiy/my-first-repository/assets/149892273/2cccfbed-eb22-40c0-bf7d-4e7bc5562437)

I'm **JavaScript developer**. *This is my example of code:*

```javascript
document.getElementById("filter-form").addEventListener("submit", function(event){
    event.preventDefault();
    sortedPokemons = pokemons
    if(event.target["name-filter"].value){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.name.indexOf(event.target["name-filter"].value.toLowerCase()) != -1
        })
    }
    if(event.target["hp-filter-form"].value > 10){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.stats[0].base_stat >= event.target["hp-filter-form"].value
        })
    }
    if(event.target["hp-filter-to"].value > 250){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.stats[0].base_stat <= event.target["hp-filter-to"].value
        })
    }
    if(event.target["attack-filter-to"].value > 5){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.stats[1].base_stat <= event.target["attack-filter-to"].value
        })
    }
    if(event.target["attack-filter-to"].value < 130){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.stats[1].base_stat <= event.target["attack-filter-to"].value
        })
    }
    if(event.target["defence-filter-to"].value > 5){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.stats[1].base_stat <= event.target["defence-filter-to"].value
        })
    }
    if(event.target["defence-filter-to"].value < 180){
        sortedPokemons = sortedPokemons.filter((pokemon)=>{
            return pokemon.stats[1].base_stat <= event.target["defence-filter-to"].value
        })
    }
    reddrawSortPokemons();
})
```

My social links
* [my instagram](https://www.instagram.com/)
* [my telegram](https://web.telegram.org/k/)
