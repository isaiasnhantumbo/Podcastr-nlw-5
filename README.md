## Exemplos de chamadas API

```
useEffect(() => {
 fetch('http://localhost:3333/episodes')
   .then((response) => response.json())
    .then((data) => console.log(data));
},[]);
```
## Chamada Api sem o axios com params
```
const response = await fetch(
    'http://localhost:3333/episodes?_limit=12&_sort=published_at&_order=desc'
  );
  const data = await response.json();
```


## Chamada Api com axios com parametros

```
const {data} = await api.get('episodes',{
  params:{
    _limit:12,
    _sort:'published_at',
    _order:'desc'
  }
})
```
### Explicação do SSG diferenças entre os fallback(blocking,true e false) - 10minuto - 
```
fallback: 'blocking'
```
Ideal para SEO

### Exemplo de SSG otimizado para os mais acessados 20:00

### Dicas finais
- PWA (next-pwa)
- Mobile layout
- Tema dark
- Electron
- 