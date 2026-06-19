method⇒the function defined in the class. comining the instance
ex)
class Car:	# carクラスの定義
    def __init__(self, brand, model):	# コンストラクタの定義
        self.brand = brand
        self.model = model

    def start(self):	# startメソッドの定義
        print(f"{self.brand} {self.model}がエンジンをかけました")

    def stop(self):		# stopメソッドの定義
        print(f"{self.brand} {self.model}が停止しました")

# Carクラスのインスタンスを2つ作成
car1 = Car("トヨタ", "プリウス")
car2 = Car("ホンダ", "シビック")

# メソッドを呼び出して、車を操作
car1.start()	# 出力: トヨタ プリウスがエンジンをかけました
car2.start()	# 出力: ホンダ シビックがエンジンをかけました

car1.stop()		# 出力: トヨタ プリウスが停止しました
car2.stop()		# 出力: ホンダ シビックが停止しました


exsecise::
# 家電製品クラスを定義します
class Appliance:
    def __init__(self, brand, power, is_on=False):
        # 家電製品のブランド、消費電力、電源の状態を定義
        self.brand = brand
        self.power = power  # 消費電力 (W)
        self.is_on = is_on  # 電源がオンかオフかの状態

    def turn_on(self):
        # 家電製品をオンにするメソッド
        if not self.is_on:
            self.is_on = True
            print(f"{self.brand}がオンになりました")
        else:
            print(f"{self.brand}は既にオンになっています")

    def turn_off(self):
        # 家電製品をオフにするメソッド
        if self.is_on:
            self.is_on = False
            print(f"{self.brand}がオフになりました")
        else:
            print(f"{self.brand}は既にオフになっています")

    def check_status(self):
        # 家電製品の電源状態を確認するメソッド
        status = "オン" if self.is_on else "オフ"
        print(f"{self.brand}の電源状態は{status}です")


# Applianceクラスのインスタンスを作成します
tv = Appliance("テレビ", 150)
fridge = Appliance("冷蔵庫", 200)

# テレビの操作
tv.check_status()	# 初期状態ではオフのはずです
tv.turn_on()		# テレビをオンにします
tv.check_status()	# 電源がオンになったか確認します
tv.turn_off()		# テレビをオフにします

# 冷蔵庫の操作
fridge.turn_on()		# 冷蔵庫をオンにします
fridge.check_status()	# 冷蔵庫の電源状態を確認します
