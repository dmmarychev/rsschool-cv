# Dzmitry Marchanka


## Contacts:
**Email:** dmmarychev@yandex.ru
**Telegram:** dmmarychev
**Mobile:** +375 (29) 344-91-54


## Experience


Period | Organization | Position 
------ | -------------| --------
april 2018 - now | Main Department of Justice of the Mogilev Oblast Executive Committee | Software engineer
august 2016- april 2018 | Mogilev city hospital of emergency medical care | Software technician



## Skills
* Framework: Foundation, UIKit, MapKit (little hands-on experience), Core Data (little hands-on experience)
* Knowledge of application lifecycle, UIViewController lifecycle
* Understanding memory management (ARC / MRC)
* Understanding the principles of OOP, SOLID, Clean code, basic design patterns
* Basic understanding of MVC, MVP, MVVM architectures
* Knowledge of iOS Human Interface Guidelines

Languages
* Objective-C
* Swift

Additional knowledge skills:
* Git (basic commands in Terminal + Github Desctop)
* Adobe XD (designing and prototyping interfaces)
* Knowledge of basic methodologies and software testing process

## Education
Period | Organization | Specialty 
------ | ------------ | ---------
2016-2020 | Belarusian-Russian University | Automated information processing systems
2012-2016 | Mogilev State Polytechnic College | Information technology software



## Code example
```Objective-C 
- (instancetype)init
{
    self = [super init];
    if (self) {
        
        _salary = 490.f;
        _averagePrice = 10.5f;
        
        [[NSNotificationCenter defaultCenter] addObserver:self
                                              selector:@selector(salaryDidChange:)
                                              name:DMGovernmentSalaryDidChangeNotification
                                              object:nil];
        
        [[NSNotificationCenter defaultCenter] addObserver:self
                                                 selector:@selector(averagePriceDidChange:)
                                                     name:DMGovernmentAveragePriceDidChangeNotification
                                                   object:nil];
    }
    return self;
}

- (void)dealloc
{
    [[NSNotificationCenter defaultCenter] removeObserver:self];
}

#pragma mark - Notifications

- (void) salaryDidChange:(NSNotification *)newSalary {
    
    float newSalaryValue = [[newSalary.userInfo objectForKey:DMGovernmentSalaryUserInfoKey] floatValue];
    
    if (newSalaryValue > _salary) {
        NSLog(@"Salary did change from %.1f to %.1f, doctor's are happy!", _salary, newSalaryValue);
    } else {
        NSLog(@"Salary did change from %.1f to %.1f, doctor's are not happy", _salary, newSalaryValue);
    }
    
    _salary = newSalaryValue;
}
```


# Knowledge of languages

English-A2
