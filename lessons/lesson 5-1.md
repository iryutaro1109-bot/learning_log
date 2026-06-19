class class name:
    variable
    def methodnome(self):

ex)
class Animal:			# Animalという名前のクラスを定義
    name = "Pochi"		# 変数nameを定義
    def speak(self):	# speakという名前のメソッドを定義 
        return "The animal makes a sound"	# メソッドの戻り値

attribute⇒the variable and method defined in the class
method⇒the function defined in the class

class⇒blue print. not active
instance(object)⇒the program made by the class

ex)
# クラス定義
class Animal:			# Animalという名前のクラスを定義
    name = "Pochi"		# 変数nameを定義
    def speak(self):	# speakという名前のメソッドを定義
        return "The animal makes a sound"

# インスタンス生成
my_animal = Animal()	# Animalクラスをインスタンス生成し、変数my_animalに代入
						# これにより、変数my_animalはAnimalクラスの実体（オブジェクト）となる

print(my_animal.name)		# 変数my_animalの中の変数nameをprintで出力
print(my_animal.speak())	# 変数my_animalの中のspeakメソッドを実行して、printで出力

__init__⇒the process of initial
constract
ex)
class Cat:						# Catクラスを定義
    def __init__(self, name):	# 引数nameを受け取るコンストラクタ（インスタンス初期化メソッド）を定義
        self.name = name		# 渡された引数nameを変数self.nameに格納する

    def speak(self):			# speakメソッドを定義
        speak = "Nyaa"			# 変数speakの定義
        return f"{self.name} says {speak}"	# 変数self.nameを使用して出力

# Catクラスのインスタンスを生成
my_cat1 = Cat("Tama")	# Tamaを引数としてCatクラスのインスタンス生成
my_cat2 = Cat("Mike")	# Mikeを引数としてCatクラスのインスタンス生成
print(my_cat1.speak())	# 出力: Tama says Nyaa
print(my_cat2.speak())	# 出力: Mike says Nyaa

i epect to used to class and __init__
