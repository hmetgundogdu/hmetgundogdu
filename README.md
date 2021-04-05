### Hi there 👋
This is Ahmet from Turkey, i love programing, tech, and such as things. I had try creating 
simple and special things  and i'm trying. Cause thats the life, we going to die and we try
to leave some things to behind us.

``` c++
class IMail() {
    public:
      virtual string GetSender() = 0;
      virtual string GetTopic() = 0;
      virtual string GetContext() = 0;
};

class IMailResult {
    public:
        virtual bool IsSuccess() = 0;
};

class MailClientBase {
  protected:
    virtual bool Auth(string host, uint16_t port, string address, string password);
    virtual IMailResult Send(MailBaseClass mail);
};

class YourMailClient : protected MailClientBase {   ...   };
class YourMail : public IMail {  ...  };

assert(new YourMailClient("fooBoo", "123456")->Send(new YourMail("hmetgundogdu@gmail.com", "", nullptr))->IsSuccess());

return 0;
```

<!--
**hmetgundogdu/hmetgundogdu** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
