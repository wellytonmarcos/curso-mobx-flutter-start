# Gerência de Estado com MobX
MobX - Modificando o Start do Flutter para Gerencia de Estado com MobX

###### Aula 1 - Criando um gerenciador de estado básico
- [x] Novo Projeto Flutter
- [x] Importação da MobX
- [x] Criação do Gerenciador de Estado
- [x] Alterando main.dart
- [x] Testando
O arquivo desta aula terá uma cópia com nome nao_utilizados/counter_aula_1.dart

###### Aula 2 - Aprimorando a Classe Counter
- [x] Importando novas dependencias
- [x] Utilizar @observable e @action
- [x] Criar um counter.g.dart com o comando "flutter packages pub run build_runner build"
- [x] Testando

### Dependencias:

Buscar as dependencias de https://pub.dev/

Em dependencias:

- MobX (https://pub.dev/packages/mobx)
- MobX Flutter (https://pub.dev/packages/flutter_mobx)


Nas dependecias de desenvolvimento: 
- MobX Codegen (https://pub.dev/packages/mobx_codegen)
- Build Runner (https://pub.dev/packages/build_runner)
(Juntos formarão um gerador de código para counter)


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


