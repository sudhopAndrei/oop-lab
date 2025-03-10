#include <iostream>

class A {
    public:
        A(){
            std::cout<<"new obj A"<<std::endl;
        };
        virtual ~A(){
            std::cout<<"delete obj A"<<std::endl;
        };
    
        void set_status(std::string newS) {
            m_status=newS;
        }
        std::string get_status(){
            return m_status;
        }
    
    private:
        std::string m_status;
};

class B : public A{
    public:
        B(){
            std::cout<<"new obj B"<<std::endl;
        };
        virtual ~B(){
            std::cout<<"delete obj B"<<std::endl;
        };
};

int main()
{
    std::cout<<sizeof(A)<<" "<<sizeof(B)<<std::endl;
    A* A_ptr=new A();
    A* B_ptr=new B();
    A_ptr->set_status("1");
    B_ptr->set_status("2");
    std::cout<<A_ptr->get_status()<<std::endl;
    std::cout<<B_ptr->get_status()<<std::endl;
    delete A_ptr;
    delete B_ptr;
}

