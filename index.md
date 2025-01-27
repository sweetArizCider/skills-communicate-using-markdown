# hellooow

Just a hellow header :)

![Vladimir from League Of Legends](https://github.com/user-attachments/assets/b0673fe1-071d-4d7e-9260-f33a0c752ecb)

- [x] Turn on GitHub Pages
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
