<p align="center">
    <a href="#">
        <img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbjWcIZ%2FbtqBc5GMjUi%2FkJsmhyQxnY0ip78okubc81%2Fimg.png" width="400">
    </a>
</p>

<p align="center">
    <strong>Kaggle Used Car Price Predict</strong>
</p>
<br>

## Way 1. Linear Regression

- checking shape
```bash
print('row 수 : {}, col 수 : {}'.format(dummy_data.shape[0], dummy_data.shape[1]))
```
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fl4IrN%2FbtqBc48X0MJ%2FRpBRCparfvOjRBaMKqhKX0%2Fimg.png" width="800">
<br>

- data preprocessing
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FeuomPK%2FbtqBc5tcPjs%2FvBkkMwkvrKkoYusDDwPNm1%2Fimg.png" width="800">
Remove Nan Causes losing lots of informations , so Drop New_Price Column, Unnamed:0 Column 

<br>
<br>
<br>

<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbKJjqy%2FbtqBdTTBPX6%2Fcs1XTVNalKVT0Gzd83ryMK%2Fimg.png" width="800">
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FdeV1eE%2FbtqBf3OgUjh%2FzNqAhnKtzrSFJrSGZKKzak%2Fimg.png" width="800">
<br>

- Generate 79 Columns
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2F6qa5E%2FbtqBeJCYkPY%2FyJIueMFr1XBuKjgmid9h4K%2Fimg.png" width="800">
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FKaUAg%2FbtqBeKIHHe3%2FWA8KnodT5MEEqDz8EK5pnK%2Fimg.png" width="800">
<br>

- Remove Outlier
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fb5N7MM%2FbtqBgdpASTr%2FLqgd7RWwn9QNWcUDRRDkik%2Fimg.png" width="800">
<br>

- Result
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbUzZcA%2FbtqBeKWfVg0%2FRYb9C2sVBaoVpjYVlVInUk%2Fimg.png" width="800">
<br>
<br>

## Way 2. Gradient Boost

- GridSearchCV()
cross validation <br>
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbAWhli%2FbtqBgEnAkcT%2FNeEkmZhYH4CRjgpCj2Qsm0%2Fimg.png" width="800">
<br>

- Result
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcA4xGr%2FbtqBeJKplZE%2F9ZyIsOAPnfyjBCX5LgFHVk%2Fimg.png" width="800">
<br>
<br>

## Way 3. Random Forest
one of Ensemble learning method, each small different decision trees make a model.
<br>

- Result
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FkLgaz%2FbtqBeTlM6Vl%2FZKjeBounPFVzQkHiEUPDhK%2Fimg.png" width="800">
<br>

## Blog Posts

- [선형회귀 Linear Regression](https://ebbnflow.tistory.com/140)
- [Gradient Boost, Random Forest](https://ebbnflow.tistory.com/141)