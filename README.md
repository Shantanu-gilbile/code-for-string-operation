# code-for-string-operation
def palindrome():
    string=input('Enter the string: ')
    a=string[-1::-1]
    if string==a:
        print('Entered String is Palindrome')
    else:
        print('Entered String is not Palindrome')


def frequency():
    string1=input('Enter the string: ')
    c=input('Enter the character to check the frequency: ')
    count=0
    for i in string1:
        if i==c:
            count+=1
    print(c,'occurs',count,'times in the above sentence')



def longestwordlength():
    sentence=input('Enter the Sentence :')
    l=0
    w=' '
    words=sentence.split()
    print(words)
    for i in words:
        if(len(i)>1):
            w=i
            l=len(i)
    print('Longest word in sentence is: ',w)
    print('Length of the word',w,'is:',l)


print('Menu')
print('1.Check wheater the string is palindrome or not.')
print('2.Check the frequency of the character') 
print('3.Check the Longest word in sentence and its length')
print('4.Exit')
l=1
while(l==1):
    ch=int(input('What you want to perform :'))
    if(ch==1):
        palindrome()
        
    elif(ch==2):
        frequency()
        
    elif(ch==3):
        longestwordlength()
        
   
    elif(ch==4):
        print('Successfully Exited.')
        break;
    else:
        print('You have entered wrong choice please check again')






