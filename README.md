#  Aplicación de web en Python

  Un cliente nos solicita una aplicación web donde tenga la vista Home, About y Contact. En
 este sentido, la solución es entregarle un ejemplo utilizando Django. Para los contenidos de
 las vistas se pueden entregar textos de prueba generados con Lorem Ipsum.
 En el caso de la vista contact, se sugiere implementar un mini formulario de contacto con
 HTML


## url.py

![url.py](https://github.com/mckateturry/appwebpython/blob/main/pantallazos/urlpantallazo.png?raw=true)


##  Crea la vista para el Home(index) de la aplicación
![url.py](https://github.com/mckateturry/appwebpython/blob/main/pantallazos/pantallazo%20(10).png?raw=true)





```html
{% extends 'base.html' %}
{% block content %}
{%load static%}


<section class="container my-5">
    <h2 class="text-center">DESTACADOS</h2>
      <hr class="linea"/>
    <div class="row g-4">
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card h-100">
          <img src="{% static 'assets/img/card1.jpg' %}" class="card-img-top img-responsive" alt="Card1" />
          <div class="card-body">
            <h5 class="card-title">Lorem ipsum dolor sit amet</h5>
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
      </div>
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card h-100">
          <img src="{% static 'assets/img/card2.jpg' %}" class="card-img-top img-responsive" alt="Card2" />
          <div class="card-body">
            <h5 class="card-title">Lorem ipsum dolor sit amet</h5>
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
      </div>
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card h-100">
          <img src="{% static 'assets/img/card3.jpg' %}" class="card-img-top img-responsive" alt="Card3" />
          <div class="card-body">
            <h5 class="card-title">Lorem ipsum dolor sit amet</h5>
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
      </div>
      <div class="col-sm-6 col-md-4 col-lg-3">
        <div class="card h-100">
          <img src="{% static 'assets/img/card4.jpg' %}" class="card-img-top img-responsive" alt="Card4" />
          <div class="card-body">
            <h5 class="card-title">Lorem ipsum dolor sit amet</h5>
            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
      </div>
    </div>
  </section>
      </div>
      </div>
        </div>
      </section>

{% endblock %}
```

##   Crea la vista para el About de la aplicación.
![url.py](https://github.com/mckateturry/appwebpython/blob/main/pantallazos/pantallazo%20(9).png?raw=true)





```html
{% extends 'base.html' %}
{% block content %}
{%load static%}


<section class="gone">
    <div class="container">
      <h2 class="text-center">¿QUIÉNES SOMOS?</h2>
      <hr class="linea"/>
      <div class="row justify-content-md-center">
  

        <div class="col1 col-sm col-lg">
            <div class="icon1"><i class="fas fa-plane"></i></div>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Odit eaque aliquam quo quibusdam ipsam voluptatem corporis soluta cum non voluptate omnis delectus aperiam autem, quia nisi distinctio ex cupiditate officia!
          Non a quod qui unde perferendis praesentium ducimus quaerat culpa rerum nobis dicta quos quam, tempore necessitatibus nemo optio quibusdam eveniet repellat et iusto consequatur fugiat veniam quisquam consectetur. At?
          Sint culpa accusamus impedit nam dolore nesciunt officia quae ducimus doloribus placeat eligendi corporis unde, accusantium ullam veritatis expedita error? Sequi quae possimus nisi accusamus assumenda tempore officiis harum libero!
        </div>
  
        <div class="col2 col-sm col-lg">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis voluptatem veritatis, pariatur nam molestias aperiam ipsum, repellendus, culpa provident consequatur quas excepturi? Optio facere exercitationem dignissimos nemo excepturi odit autem.
          Adipisci totam similique voluptas culpa! Neque accusantium voluptatum distinctio dicta rem excepturi delectus velit quae possimus corporis. Nobis quis explicabo praesentium recusandae ipsum ut. Voluptate quidem dolorem praesentium pariatur perspiciatis!
          Quidem autem ipsa illo nam id nesciunt harum amet exercitationem ab consequuntur. Eum iste temporibus qui nulla expedita recusandae vel doloremque, impedit libero quas repellendus ipsa aliquid minus dolore. Saepe.
          <div class="icon2"><i class="fas fa-mountain"></i></div>
        </div>
  
        <div class="col3 col-sm col-lg">
          <div class="icon1"><i class="fas fa-route"></i></div>           
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia unde reprehenderit magni omnis, maxime, architecto iusto deserunt animi nostrum inventore nesciunt magnam explicabo natus illo. Repudiandae sit fugiat cupiditate omnis.
          Quae voluptatum aliquam atque rerum nemo omnis magnam ab odit animi. Ducimus, deserunt vel inventore fugiat corrupti nemo saepe nisi cupiditate voluptate vitae delectus ea ipsa. Hic officiis enim nobis.
          Officia quibusdam rem suscipit provident consectetur doloribus enim eum sed? Temporibus et esse natus ullam fugit! Rerum id temporibus iste fuga, sit, dolores laudantium eos quisquam molestiae, eius corporis error.
        </div>
      </div>
    </div>
  </section>



{% endblock %}
```


##   Crea la vista para contact de la aplicación.
![url.py](https://github.com/mckateturry/appwebpython/blob/main/pantallazos/pantallazo%20(1).png?raw=true)





```html
{% extends 'base.html' %}
{% block content %}
{%load static%}

<section id="form-section">
    <div class="form-container">
      <form action="" method="post">
        <h2 class="text-center mb-4">CONTACTO</h2>
        <div class="mb-3">
          <label for="form-input-nombre" class="form-label">Nombre</label>
          <input type="text" class="form-control" id="form-input-nombre" />
        </div>
        <div class="mb-3">
          <label for="form-input-asunto" class="form-label">Asunto</label>
          <input type="text" class="form-control" id="form-input-asunto" />
        </div>
        <div class="mb-3">
          <label for="form-textarea-mensaje" class="form-label">Mensaje</label>
          <textarea class="form-control" id="form-textarea-mensaje" data-bs-custom-class="custom-tooltip" data-bs-toggle="tooltip" data-bs-placement="bottom" title="Consulte por nuestras promociones y descuentos" rows="3"></textarea>
        </div>
        <div class="mb-3 text-center">
          <button id="enviarFormulario" type="submit" class="btn btn-lg bg-viajes text-white mb-3 border-0 bg-opacity-75">Enviar</button>
        </div>
      </form>
    </div>
  </section>


  {% endblock %}
```
