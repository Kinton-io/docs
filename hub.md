# Hub


Como ya se ha visto, *Kinton* usa *MQTT* para la comunicación entre los dispositivos y aplicaciones con el _broker_, sin embargo, no todos los dispositivos son capaces de usar *MQTT* o, simplemente, son dispositivos cuyo _firmware_ no puede ser modificado para que sea compatible con *Kinton*.

Para poder conectar dispositivos que, en principio, no son compatibles con la arquitectura de *Kinton* se puede utilizar un elemento intermedio que actúe como intermediario entre el _broker_ y el dispositivo incompatible. 

```flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|request

st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e

```

{% flow %}
st=>start: Start:>http://www.google.com[blank]
e=>end:>http://www.google.com
op1=>operation: My Operation
sub1=>subroutine: My Subroutine
cond=>condition: Yes
or No?:>http://www.google.com
io=>inputoutput: catch something...

st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
{% endflow %}

