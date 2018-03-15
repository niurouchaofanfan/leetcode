# leetcode
bool isPalindrome(int x) {
    int z=x;
    int y=0;
    if(x<10 && x>=0){
        return true;
    }else if(x<0 || x%10==0){
        return false;
    }
    while(x!=0){
        y=y*10 + x%10;
        x=x/10;
    }
    if(fabs(z-y)<1e-3){
        return true;
    }else
        return false;
}
