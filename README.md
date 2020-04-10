# Gerência de Estado com MobX
MobX - Modificando o Start do Flutter para Gerencia de Estado com MobX

- [x] Novo Projeto Flutter
- [x] Importação da MobX
- [x] Criação do Gerenciador de Estado
- [x] Alterando main.dart
- [x] Testando

### Dependencias:
Buscar as dependencias de https://pub.dev/
- MobX (https://pub.dev/packages/mobx)
- MobX Flutter (https://pub.dev/packages/flutter_mobx)

### Arquivo de Gerencia
- counter.dart

### Modificar Main.dart
- remover setState()
- Adicionar Counter
```
  Counter counter = Counter();
```
- Ajustar Clique do botão 
```
  onPressed: counter.increment,
```
- Ajustar Text para dentro do Observer
```
  Observer(
      builder: (_)
      {
        return Text(
          '${counter.count}',
          style: Theme.of(context).textTheme.display1,
        );
      }
    ),
```


