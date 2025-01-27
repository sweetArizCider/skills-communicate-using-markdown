# HI!!
 I'm **Ariz**, I'm 20, and I'm pretty interested in **WEB DEVELOPMENT** and **MUSIC**
 
![Vladimir _ League of Legends](https://github.com/user-attachments/assets/6139ad90-4c6f-4ca9-8aad-336c1ab7ef86)

- [x] Turn on GitHub Pages
- [x] Learning Javascript
- [x] Learning Css
- [ ] Outline my portfolio
- [ ] Introduce myself to the world
- [x] Listen Mattmaltese

``` javascript
const Joi = require('joi')

class AutoresValidations{

    validateAutorRegister(autor_data){
        const schema = Joi.object({
            nombre: Joi.string()
                .pattern(new RegExp('^[áéíóúÁÉÍÓÚa-zA-ZÑñ]{3,15}$')) 
                .required(),
            apellidoPaterno: Joi.string()
                .pattern(new RegExp('^[áéíóúÁÉÍÓÚa-zA-ZÑñ]{3,15}$')) 
                .required(),
            apellidoMaterno: Joi.string()
                .pattern(new RegExp('^[áéíóúÁÉÍÓÚa-zA-ZÑñ]{3,15}$')) 
                .required()
        });

        return schema.validate(autor_data)
    }

    
}

module.exports = AutoresValidations;
```
