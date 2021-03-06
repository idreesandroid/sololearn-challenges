# OneLiners solutions in Ruby

There is Ruby's #OneLiners solutions for Sololearn Code Coach challenges. 
All of the solutions have passed the tests in Sololearn. Currently there are 61 out of 72 or 85% of code challenges that I can solve in one line of code.

## Easy

[Popsicles](easy/popsicles/README.md)

```ruby
puts [gets.to_i, gets.to_i].reverse.inject(:%) == 0 ? 'give away' : 'eat them yourself'
```

[Halloween Candy](easy/halloween-candy/README.md)

```ruby
puts (100 * 2.0 / gets.to_i).ceil
```

[Fruit Bowl](easy/fruit-bowl/README.md)
```ruby
puts gets.to_i / 6
```

[Ballpark Orders](easy/pro-ballpark-orders/README.md)

```ruby
puts '%.2f' % [((menu={Nachos: 6, Pizza: 6, Cheeseburger: 10, Water: 4, Coke: 5}).default = menu[:Coke]), gets.split.map {|i| menu[i.to_sym]*1.07}.inject(:+)][1]
```

[Skee-ball](easy/skee-ball/README.md)

```ruby
puts gets.to_i / 12 >= gets.to_i ? "Buy it!" : "Try again"
```

[Paint Costs](easy/paint-costs/README.md)

```ruby
puts (1.1 * (5 * gets.to_i + 40)).round
```

[Argentina](easy/argentina/README.md)

```ruby
puts gets.to_i < gets.to_i * 50 ? "Pesos" : "Dollars"
```

[Balconies](easy/pro-balconies/README.md)

```ruby
puts "Apartment " + (Array.new(2){gets.split(",").map(&:to_i).inject(:*)}.inject(:>) ? "A": "B")
```

[Candles](easy/pro-candles/README.md)

```ruby
puts 9 * gets.to_i + 9
```

[Duct Tape](/easy/pro-duct-tape/README.md)

```ruby
puts (2.0 * gets.to_i * gets.to_i / 10).ceil
```

[Easter Eggs](easy/pro-easter-eggs/README.md)

```ruby
puts gets.to_i > gets.to_i + gets.to_i ? 'Keep Hunting' : 'Candy Time'
```

[Guard Flamingos](easy/guard-flamingos/README.md)

```ruby
puts gets.to_i + gets.to_i
```
[Gotham City](easy/gotham-city/README.md) 

```ruby
puts ["I got this!", "Help me Batman", "Good Luck out there!"][((gets.to_i-5)/6<=>0)+1]
```

[Hovercraft](easy/hovercraft/README.md)

```ruby
puts ['Loss','Broke Even','Profit'][1+(gets.to_i<=>7)]
```

[Izzy the Iguana](easy/pro-izzy-the-iguana/README.md)
```ruby
puts gets.split.map {|item| {Lettuce: 5, Carrot: 4, Mango: 9, Cheeseburger: 0}[item.to_sym]}.inject(:+) >= 10 ? 'Come on Down!' : 'Time to wait'
```

[Jungle Camping](easy/jungle-camping/README.md)

```ruby
puts gets.split.map{|sound| {Grr:"Lion",Rawr:"Tiger",Ssss:"Snake",Chirp:"Bird"}[sound.to_sym]}.join(' ')
```

[Land Ho!](easy/pro-land-ho/README.md)
```ruby
puts gets.to_i / 20 * 20 + 10
```

[Neverland](easy/pro-neverland/README.md)

```ruby
puts 'My twin is %d years old and they are %d years older than me' % [gets.to_i + y = gets.to_i, y]
```

[Extra-Terrestrials](easy/extra-terristrials/README.md)
```ruby
puts gets.reverse
```

[Zip Code Validator](easy/pro-zip-code-validator/README.md)
```ruby
puts nil!=(gets=~/^\d{5}$/)
```

[Vowel Counter](easy/pro-vowel-counter/README.md)
```ruby
puts gets.gsub(/[^AEIOUaeiou]/, '').size
```

[Isogram Detector](easy/pro-isogram-detector/README.md)

```ruby
puts gets.match(/(.).*\1/) == nil
```

[Multiples](easy/pro-multiples/README.md)

```ruby
puts (0...gets.to_i).filter {|i| i % 3 == 0 || i % 5 == 0}.inject(:+)
```

[Number of Ones](easy/pro-number-of-ones/README.md)

```ruby
puts gets.to_i.to_s(2).gsub(/0/,'').size
```


## Medium

[Pig Latin](medium/pig-latin/README.md) 
```ruby
puts gets.split.map {|w| w[1,w.size] + w[0] + 'ay'}.join(' ')
```

[Safety Deposit Boxes](medium/pro-safety-deposit-boxes/README.md) 

```ruby
puts gets.chomp.split(',').index(gets) * 5 + 5
```

[Roadrunner](medium/pro-roadrunner/README.md)

```ruby
puts [t=(s=gets.to_f)/gets.to_i,gets.to_i>(50+s)/t ?'Yum': 'Meep Meep'][1]
```

[Snap, Crackle and Pop](medium/pro-snap-crackle-and-pop/README.md)

```ruby
puts Array.new(6){gets.to_i}.map{|i| i % 3 > 0 ? i % 2 > 0 ? "Snap" : "Crackle" : "Pop"}.join(' ')
```

[Deja Vu](medium/deja-vu/README.md)

```ruby
puts gets =~ /(.).*\1/ ? 'Deja Vu' : 'Unique'
```

[The Spy Life](medium/the-spy-life/README.md)

```ruby
puts gets.gsub(/[^A-Za-z ]/, '').reverse
```

[Hex Color Code Generator](medium/pro-hex-color-code-generator/README.md) 

```ruby
printf("#%02x%02x%02x", gets.to_i, gets.to_i, gets.to_i)
```

[Symbols](medium/symbols/README.md)

```ruby
puts gets.gsub(/[^A-Za-z 0-9]/, '')
```

[Carrot Cake](medium/pro-carrot-cake/README.md)

```ruby
puts [7 - gets.to_i % gets.to_i].map{|x| x > 0 ? 'I need to buy %d more' % x : 'Cake Time'}
```

[Super Sale](medium/pro-super-sale/README.md)

```ruby
puts (1.07 * 0.30 * gets.split(',').map(&:to_f).sort.reverse.drop(1).push(0).inject(:+)).to_i
```

[Duty Free](medium/pro-duty-free/README.md)

```ruby
puts gets.split.map(&:to_f).any?{|x| 20 < 1.1 * x} ? 'Back to the store': 'On to the terminal'
```

[Building Blocks](medium/pro-building-blocks/README.md)

```ruby
puts Array.new(4){gets.to_i % 15}.inject(:+)
```

[Name Buddy](medium/pro-name-buddy/README.md)

```ruby
puts gets.chomp + ' ' + gets =~ /\b(\w).*\b\1\w*$/ ? 'Compare notes' : 'No such luck'
```

[That's odd...](medium/thats-odd/README.md) 

```ruby
puts Array.new(gets.to_i){gets.to_i}.select(&:even?).push(0).inject(:+)
```

[No Numerals](medium/no-numerals/README.md)

```ruby
puts gets.split.map{|w| w=~/1?\d/ ? ['zero','one','two','three','four','five','six','seven','eight','nine','ten'][w.to_i]: w}.join(' ')
```

[Secret Message](medium/secret-message/README.md) 

```ruby
puts gets.downcase.chars.map{|c| c=~/^[a-z]$/?('az'.sum-c.ord).chr: c}.join
```

[Divisible](medium/pro-divisible/README.md)

```ruby
puts [n=gets.to_i,gets.split.map(&:to_i).any?{|x| n%x>0} ? 'not divisible by all': 'divisible by all'][1]
```

[Even Numbers](medium/pro-even-numbers/README.md)

```ruby
puts gets.split.map(&:to_i).select(&:even?).join(' ')
```

[Tax Free](medium/pro-tax-free/README.md) 

```ruby
puts gets.split(',').map(&:to_f).map{|x| x < 20 ? 1.07 * x : x}.inject(:+)
```

[How Far?](medium/pro-how-far/README.md)

```ruby
puts gets.gsub(/^B*[HP](B*)[HP]B*$/,'\1').size
```

[Average Word Length](medium/average-word-length/README.md)

```ruby
puts ((essay=gets).gsub(/[^a-zA-Z]+/,'').size.to_f / essay.split.size).ceil
```

[YouTube Link Finder](medium/youtube-link-finder/README.md)

```ruby
puts gets.gsub(/.*[=\/](?=[^=\/]*$)/, '')
```

[Camel to Snake](medium/pro-camel-to-snake/README.md) 

```ruby
puts gets.gsub(/(?<=[^\/b])([A-Z])/, '_\1').downcase
```

[Text Decompressor](medium/pro-text-decompressor/README.md)

```ruby
puts gets.split(/(?<=\d)/).map{|x| x[0] * x[1].to_i}.join()
```

[Snowballing Numbers](medium/pro-snowballing-numbers/README.md) 

```ruby
puts 0 < Array.new(gets.to_i){gets.to_i}.reduce{|a,b| a > 0 && b > a ? a + b : 0}
```

[Flowing Words](medium/pro-flowing-words/README.md)

```ruby
puts nil!=(gets =~/^(\S*(\S) \2\S*)*$/)
```

[Splitting Strings](medium/pro-splitting-strings/README.md)

```ruby
puts gets.chomp.split(Regexp.new '(?<=\G.{%d})' % gets.to_i).join('-')
```

[Missing Numbers](medium/pro-missing-numbers/README.md)

```ruby
print ((a=Array.new(gets.to_i){gets.to_i})[0].upto(a[-1]).to_a - a).join(' ')
```

[Initials](medium/pro-initials/README.md)

```ruby
puts Array.new(gets.to_i){gets.chomp.gsub(/(\w)\w* (\w)\w*/,'\1\2')}.join(' ')
```

[Credit Card Validator](medium/pro-credit-card-validator/README.md)

```ruby
puts (n=gets).size == 16 && n.reverse.chars.map(&:to_i).map.with_index{|x,i| i.odd?? x>4 ? x*2-9: x*2: x}.sum%10==0 ? 'valid': 'not valid'
```

[CMYK to RGB](medium/pro-CMYK-to-RGB/README.md)

```ruby
puts '%d,%d,%d' % (a=Array.new(4){1-gets.to_f}).first(3).map{|x| (255*x*a.last).round}
```

## Hard

[New Driver's License](hard/new-drivers-license/README.md)

```ruby
puts [hero=gets, agents=gets.to_i, 20 * (1 + gets.split.select{|name| name < hero}.size / agents)][2]
```

[It's a Sign](hard/pro-its-a-sign/README.md)

```ruby
puts Array.new(4){gets.chomp}.any?{|s| s == s.reverse} ? 'Open' : 'Trash'
```

[Password Validation](hard/password-validation/README.md)

```ruby
puts [gets].map{|x| x.length > 6 && x =~ /\d.*\d/ && x =~ /([!@#$%&*].*){2,}/ ? "Strong": "Weak"}
```

[Security](hard/security/README.md)

```ruby
puts gets =~ /[$T].*G.*[$T]/ ? 'quiet': 'ALARM'
```

[2D Map](hard/pro-2d-map/README.md)

```ruby
puts (b=(m=gets).index('P',1+a=m.index('P')))/6-a/6+(a%6-b%6).abs
```

[Hofstadter's Q-Sequence](hard/pro-hofstadter-q-sequence/README.md)

```ruby
puts [q=Array.new(2,1),2.upto(gets.to_i-1){|i| q<<q[i-q.last]+q[i-q[i-2]]},q.last].last
```
_The one-liner is equals to the following code:_
```ruby
def Q(n)
   q = Array.new(2, 1)
   2.upto(n - 1){|i| q << q[i - q.last] + q[i - q[i - 2]]}
   return q.last
end
n = gets.to_i
puts Q(n)
```

[Digits of Pi](hard/pro-digits-of-pi/README.md)

_Using the fact that required digits of pi limited by 1000 this problem can be solved by coping first 1000 pi digits from Wikipedia and writing one-liner like this:_

```ruby
puts '.1415926...'[gets.to_i]
```
You can check program in python that uses this approach: [DigitsPi.py](hard/pro-digits-of-pi/DigitsPi.py)

Hovewer there is program to compute pi digits by using The Gauss–Legendre iterative algorithm:

```ruby
require 'bigdecimal'

# The Gauss–Legendre iterative algorithm

def calculatePi(precision = 800)
   # The algorithm has quadratic convergence, which essentially means that
   # the number of correct digits doubles with each iteration of the algorithm.
   BigDecimal.limit(precision);
   
   one = BigDecimal(1)
   two = BigDecimal(2)
   four = BigDecimal(4)
   
   # Initial value setting:
   a = one
   b = one / two.sqrt(precision)
   t = one / four
   p = one
   
   # Repeat the following instructions until 
   # the difference of a and b is within the desired accuracy:
   c = one / 10 ** precision
   
   until (a - b).abs <= c do
       an = (a + b) / two
       bn = (a * b).sqrt(precision)
       tn = t - (p * ((a - an) ** two))
       pn = two * p
       
       a = an
       b = bn
       t = tn
       p = pn
   end
   
   # π is then approximated as:
   ((a + b) ** 2) / (t * four)
end

n = gets.to_i + 2
pi = calculatePi(n).to_s

puts pi[n]
```
