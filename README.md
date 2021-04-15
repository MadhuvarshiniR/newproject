# newproject
Infytq Practice Problems:

def check_anagram(data1,data2):
    #start writing your code here
    data1=data1.lower()
    data2=data2.lower()
    ans=[]
    if len(data1)==len(data2):
        for i in range(0,len(data1)):
            if data1[i] in data2 and data2[i] in data1 and data1[i]!=data2[i]:
                print(data1[i],data2[i])
                ans.append(1)
    if len(ans)==len(data1):
        return True
    else:
        return False
    
print(check_anagram("eat","tea"))
