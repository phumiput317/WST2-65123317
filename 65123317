class Person {
  String _name = '';
  String get name => _name;
  set name(String value) => _name = value;
}

class Engine {
  String _model = "";
  String _speed = "0"; 
  String get model => _model;
  set model(String value) => _model = value;
  String get speed => _speed; 
  set speed(String value) => _speed = value; 

  void displayEngineInfo() {
    print('  Engine Model: $model');
    print('  Engine Speed: $speed km/h');
  }
}

class Car {
  String _brand = "";
  String _model = "";
  Person _owner;
  Engine _engine;

  Car({
    required String brand,
    required String model,
    required Person owner,
    required Engine engine,
  })  : _brand = brand,
        _model = model,
        _owner = owner,
        _engine = engine;

  String get brand => _brand;
  set brand(String value) => _brand = value;

  String get model => _model;
  set model(String value) => _model = value;

  Person get owner => _owner;
  set owner(Person value) => _owner = value;

  Engine get engine => _engine;
  set engine(Engine value) => _engine = value;

  void displayCarInfo() {
    print('Car Information:');
    print('  Brand: $brand');
    print('  Model: $model');
    print('  Owner: ${owner.name}');
    print('  Engine Information:');
    engine.displayEngineInfo();
  }

  void run() {
    print('The car is running at ${engine.speed} km/h.');
  }
}

class Honda extends Car {
  String _color = "";

  Honda({
    required String brand,
    required String model,
    required Person owner,
    required Engine engine,
    required String color,
  }) : super(brand: brand, model: model, owner: owner, engine: engine) {
    _color = color;
  }

  String get color => _color;
  set color(String value) => _color = value;

  void displayCarInfo() {
    print('Car Information:');
    print('  Brand: $brand');
    print('  Model: $model');
    print('  Color: $color');
    print('  Owner: ${owner.name}');
    print('  Engine Information:');
    engine.displayEngineInfo();
  }

  void run() {
    print('The Honda is running at ${engine.speed} km/h.');
  }
}

void main() {
  Person owner = Person();
  owner.name = 'John Doe';

  Engine engine = Engine();
  engine.model = 'V6';
  engine.speed = '120'; 

  Honda honda = Honda(
    brand: 'Honda',
    model: 'Civic',
    owner: owner,
    engine: engine,
    color: 'Red',
  );

  honda.displayCarInfo();
  honda.run();
}
