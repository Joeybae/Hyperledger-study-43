# Hyperledger-study-43

하이퍼레져 앱 만들기 실습 43일차 - split, replace, Number, toFixed

1. Awair - 기본 데이터

        var Awair = {
        "data":[
        {"timestamp":"2019-10-30T08:58:22.516Z",
        "score":85.0,
        "sensors":[
        {"comp":"temp","value":23.020000457763672},
        {"comp":"humid","value":46.220001220703125},
        {"comp":"co2","value":1487.0},
        {"comp":"voc","value":356.0},
        {"comp":"pm25","value":2.0}],
        "indices":[{"comp":"temp","value":0.0},{"comp":"humid","value":0.0},{"comp":"co2","value":2.0},{"comp":"voc","value":1.0},{"comp":"pm25","value":0.0}]}]
        }

2. split - 문자열 자르는 함수

        # var split = Awair.split('"');

        var split ={
        "data":[{"timestamp":"2019-10-30T07:11:45.226Z","score":85.0,"sensors":[{"comp":"temp","value":22.469999313354492},{"comp":"humid","value":47.38999938964844},{"comp":"co2","value":1519.0},{"comp":"voc","value":350.0},{"comp":"pm25","value":3.0}],"indices":[{"comp":"temp","value":0.0},{"comp":"humid","value":0.0},{"comp":"co2","value":3.0},{"comp":"voc","value":1.0},{"comp":"pm25","value":0.0}]}]
        }

3. replace - 특정 문자 제거하는 함수

        # split[16] = :22.469999313354492},{
        # var replace = split[16].replace('},{',"").replace(':',"") //22.469999313354492
        # 22.469999313354492 = 문자(string)

4. Number - 문자를 숫자로 바꾸는 함수

        # var num = Number(replace) //22.469999313354492
        # 22.469999313354492 = 숫자(number)

5. toFixed - 소수점의 개수를 조정하는 함수

        # var tofixed = num.toFixed(1) //22.4
        # toFixed 함수를 사용하기 위해서는 문자를 숫자로 변경해야한다.
