### Hi there 👋
Hi, I'm Ahmet from Turkey. I'm passionate about programming and technology. I enjoy building simple yet impactful projects, always striving to create something meaningful. Life is short, and while we're here, I believe it's important to leave a positive mark behind.

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

assert(!(
	    new YourMailClient("fooBoo", "123456")
	        ->Send(new YourMail("hmetgundogdu@gmail.com", "", nullptr))
	        ->IsSuccess()
	    )
    );

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
