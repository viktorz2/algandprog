# Алгоритмизация и программирование
Автор: Зубарчук Виктор
Контест 1 [https://contest.yandex.ru/contest/52142/problems/] :
 1. Приближенное значение Пи
          #include <iostream>
          #include <math.h>
          using namespace std;
          int main(){
            double pi;
            double a{ sqrt(12) };
            double b;
            b = 1.0 - (1.0 / pow(3, 2)) + (1.0 / (5 * pow(3, 2))) - (1.0 / (7 * pow(3, 3))) + (1.0 / (9 * pow(3, 4))) - (1.0 / (11 * pow(3, 5)));
            pi = a * b;
            std::cout << pi << std::endl;
            }
 2. Кислород
          package main
          import "fmt"
          func main() {
              var chel float32=0.5*365
              var dub float32=20
              var top float32=32
              var koltop float32=chel/top
              var koldub float32=chel/dub
              var t int = int(koltop)+1
              var d int = int(koldub)+1
              fmt.Print(chel,t,d)
          }
 3. Частное
          #include <iostream>
          #include <math.h>
          using namespace std;
          int main(){
          double a;
          double b;
          std::cin >> a >> b;
          std::cout << a/b << std::endl;
          }
 4. Произведение
          package main
          import "fmt"
          func main() {
              var a,b int
              fmt.Scan(&a, &b)
              var c int=a*b
              fmt.Println(c)
          }
 5. Индекс масссы тела
          #include <iostream>
          #include <math.h>
          using namespace std;
          int main(){
              double i;
              double m;
              double h;
              std::cin >> m >> h;
              i=m/pow(h,2);
              std::cout << i << std::endl;
          }
 6. Банкомат
          package main
          import "fmt"
          func main() {
              var n int
              var k5000,k1000,k500,k200,k100 int
              fmt.Scan(&n)
              for n>=5000{
                  k5000++
                  n=n-5000
              }
              for n<5000&&n>999{
                  k1000++
                  n=n-1000
              }
              for n<1000 && n>499{
                  k500++
                  n-=500
              }
               for n<500 && n>199{
                  k200++
                  n-=200
              }
              for n<200 && n>99{
                  k100++
                  n-=100
              }
          fmt.Println(k5000,k1000,k500,k200,k100)    
          }
 7. Максимум из двух чисел
          #include <stdio.h>
          #include <math.h>
          #include <iostream>
          int main(){
              int a,b;
              std::cin >> a>>b;
              if (a>b){
                  std::cout << a << std::endl;
              }
              else {
                  std::cout << b << std::endl;
              }
          }
 8. Максимум из трёх чисел
          package main
          import "fmt"
          func main() {
              var a,b,c int
              fmt.Scan(&a,&b,&c)
              if a>b{
                  if a>c{
                      fmt.Println(a)
                  } else {
                      fmt.Println(c)
                  }
                  }else{
                  if b>c{
                      fmt.Println(b)
                  } else{
                      fmt.Println(c)
                  }
              }
          }
 9. Длина гипотенузы
          #include <stdio.h>
          #include <math.h>
          #include <iostream>
          int main()
          {
              double a,b,c;
              std::cin >> a>> b;
              c=sqrt(pow(a,2)+pow(b,2));
              std::cout << c << std::endl;
          }
 10. Дерево решений
          package main
          import "fmt"
          func main() {
              var pl, kr, dlh string
              fmt.Scan(&pl,&kr,&dlh)
              if pl=="Нет" && kr=="Нет"&& dlh=="Нет" {
                 fmt.Println("Кот")
              } else if pl=="Нет" && kr=="Нет"&& dlh=="Да"{
                  fmt.Println("Жираф")
              }else if pl=="Нет" && kr=="Да"&& dlh=="Нет"{
                  fmt.Println("Курица")
              }else if pl=="Нет" && kr=="Да"&& dlh=="Да"{
                  fmt.Println("Страус")
              }else if pl=="Да" && kr=="Нет"&& dlh=="Нет"{
                  fmt.Println("Дельфин")
              }else if pl=="Да" && kr=="Нет"&& dlh=="Да"{
                  fmt.Println("Плезиозавры")
              }else if pl=="Да" && kr=="Да"&& dlh=="Нет"{
                  fmt.Println("Пингвин")
              }else if pl=="Да" && kr=="Да"&& dlh=="Да"{
                  fmt.Println("Утка")
              }    
          }
 11. Ближайшая из трёх точек
          #include <stdio.h>
          #include <math.h>
          #include <iostream>
          int main(){
              int a,b,c;
              std::cin >> a>>b>>c;
              int ab,ac;
              ab=abs(a-b);
              ac=abs(a-c);
              ab<ac ? std::cout << "B"<< "\t"<<ab: std::cout << "C"<< "\t"<<ac;
          }
 12. Гипотеза Коллатца
          package main
          import "fmt"
          func main() {
              var x,k int
              fmt.Scan(&x)
              for ;x>1;{
                  if (x%2==0 && x!=1){
                      x=x/2
                      k+=1
                  }else{
                      x=3*x+1
                      k+=1 
                  }
              }
              fmt.Println(k)  
          }
 13. Вывод чисел волнами
          #include <iostream>
          #include <math.h>
          using namespace std; 
          int main()
          {
              int n;
              int k=1;
              cin>>n;
              int maxl=2, nowl=1, step=1;
              for (int i=0;i<n;i++){
                  for (int j=0; j<nowl;j++){
                      cout<<k<<" ";
                      if (k==n){
                          n-=1000;
                          break;
                      }
                      k++;
                  }
                  nowl+=step;
                  cout<<"\n";
                  if (nowl==maxl){
                      step=-1;
                      maxl++;
                  }
                  if (nowl==1){
                      step=1;
                  }
              }  
          }
 14. Таблица умножения
          package main
          import "fmt"
          func main() {
            var row, col int
            fmt.Scan(&col, &row)
            fmt.Printf("%4v","    |")
            for i := 1; i <= row; i++ {
                 fmt.Printf("%4v", i)
            }
            fmt.Print("\n   --")
            for i := 1; i <= row; i++ {
              fmt.Printf("----")
            }
            fmt.Print("\n")
            for i := 1; i <= col; i++ {
              fmt.Printf("%4v|", i)
            for j := 1; j <= row; j++ {
              fmt.Printf("%4v", i*j)
            }
            fmt.Print("\n")
            }
          }
 15. RLE сжатие
          #include <iostream>
          #include <math.h>
          using namespace std;
          int main()
          {
              int k=1;
              string s1,s;
              cin>>s1;
              s=s1+"0";
              char last=s[0];
              for (int i=1; i<s.length();i++){
                  if(s[i]==last){
                      k++;
                  }
                  if(s[i]!=last){
                      cout<<last;
                      if (k>1){
                          cout<<k;
                      }
                      k=1;
                      last=s[i];
                  }
              }
          }
 16. Сглаживание графика погоды
          package main
          import "fmt"
          func main() {
              var lot int
              fmt.Scan(&lot)
              var masnum[] float32
              var num,res float32
              for i:=0; i<lot; i++{
                  fmt.Scan(&num)
                  masnum=append(masnum, num)
              }
              for j:=0; j<lot;j++{
                  if j==0{
                      fmt.Print(masnum[j]," ")
                  }
                  if j>0 && j<(lot-1){
                      res=(masnum[j-1]+masnum[j]+masnum[j+1])/3
                      fmt.Print(res," ")
                  }
                  if j==(lot-1){
                      fmt.Print(masnum[j])
                  }
              }
          }
 20. Анаграмма. 2 числа
          #include <iostream>
          #include <cmath>
          using namespace std;
          int main(){
              string num1,num2;
              cin >> num1>>num2;
              int k=0;
              for (int i=0;i<num1.length();i++){
                  for (int j=0;j<num1.length();j++){
                      if(num1[i]==num2[j]){
                          k++;
                          break;
                      }
                  }
              }
              if (k==num1.length()){
                  cout<<"YES";
              }
              else{
                  cout<<"NO";
              }
          }
Контест 2 [https://contest.yandex.ru/contest/52676/problems/] :
  1. Функция. Простое число
          #include <iostream>
          #include <cmath>
          using namespace std;
          bool is_prime(int x){
              int k=9;
              for (int i=2; i<=sqrt(x); i++){
                  if(x%i==0){
                      k=1;
                      break;
                  }
              }
              if (k==9){
                  return true;
              }
              else{
                  return false;
              }
          }
  2. Функция. Выход из лабиринта
          struct Point {
            int row;
            int col;
          };
          bool is_can_exit_from_maze(std::vector<std::string> maze, int start_row, int start_col){
            std::vector<Point> should_visit;
            should_visit.push_back({start_row, start_col});
            while (!should_visit.empty()) {
              Point current_point = should_visit.back();
              if (maze[current_point.row][current_point.col] == 'E') {
                return true;
              }
              should_visit.pop_back();
              // Check left
              if (current_point.col > 0 && maze[current_point.row][current_point.col - 1] != '#') {
                should_visit.push_back({current_point.row, current_point.col - 1});
              }
              // Check right
              if (current_point.col < maze[current_point.row].length() - 1 && maze[current_point.row][current_point.col + 1] != '#') {
                should_visit.push_back({current_point.row, current_point.col + 1});
              }
              // Check forward
              if (current_point.row > 0 && maze[current_point.row - 1][current_point.col] != '#') {
                should_visit.push_back({current_point.row - 1, current_point.col});
              }
              // Check back
              if (current_point.row < maze.size() - 1 && maze[current_point.row + 1][current_point.col] != '#') {
                should_visit.push_back({current_point.row + 1, current_point.col});
              }
              maze[current_point.row][current_point.col] = '#';
            }
            return false;
          }
     



