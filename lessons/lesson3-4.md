high stair function
ex)
def greet(name):	# 関数greetの定義
    return f"Hello, {name}!"

def call_function(func, name):	# 2つの仮引数を持つ関数call_functionの定義
    return func(name)

# 引数として関数を渡す
print(call_function(greet, "Bob"))	# 関数call_functionの実引数として関数greetを渡す

ambiguous
