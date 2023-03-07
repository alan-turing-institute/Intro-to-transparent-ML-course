# Machine learning process

Machine learning process can be described in terms of lifecycle phases. The phases of a machine learning system’s lifecycle are a number of analytically distinct activities throughout the stages of system design, development, and deployment. There is no universally agreed breakdown of lifecycle phases for machine learning systems but they generally follow the same [systems development life cycle](https://en.wikipedia.org/wiki/Systems_development_life_cycle) shown below as other software systems:

```{figure} https://upload.wikimedia.org/wikipedia/commons/7/7e/SDLC-Maintenance-Highlighted.png
---
name: SDLC-Maintenance-Highlighted
width: 300px
---
A general systems development life cycle, from Wikipedia.
```

## Lifecycle phases for design & development:

Below are the typical lifecycle phases for design and development of machine learning systems. Although they are expressed in business terms, they can be easily adapted to your research context!

- **Business case and problem definition**: Establishing the need for the ML system and the tasks it is meant to perform.
- **System requirements specification**: Translating the problem definition into technical design and performance requirements.
- **Data acquisition and preparation**: Where relevant, acquiring any data that may be needed to build the system, checking its suitability, and preparing it for use, e.g. via data pre-processing and/or data augmentation.
- **Building**: Creating a system that meets the design requirements previously specified. In the case of ML projects, this involves choosing between ML methods, developing and evaluating candidate models, and selecting the best performing model.
- **Validation and verification**: Verifying, on an on-going basis, that the system meets the relevant design and performance requirements. Depending on the nature of the system, assessment can rely on empirical testing or formal verification.

## Lifecycle phases for system deployment

- **Integration**: Preparing the ML system for operation by integrating it into the relevant real-world (e.g. business) environment. This can involve technical aspects of integration with other systems or technology infrastructure. It also includes the introduction of users to the operation of the system, the delivery of user training, and other relevant aspects of organisational change management.
- **Operation**: Using the ML system to perform the real-world (e.g. business) tasks for which it was intended.
- **Monitoring and evaluation**: Observing and recording system behaviour in order to assess system performance and compliance during operation, including any procedures of periodic re-validation.
- **Updating/system retirement**: Making changes to the ML system as needed, for example to improve performance or prevent performance deterioration. In the context of supervised ML models, such changes take the form of retraining the model based on new training data. Successful updating is followed by another iteration of lifecycle steps outlined above.

## Execution of lifecycle phases

The lifecycle phases capture activities that are conceptually distinct, but do not necessarily occur in succession. During an ML system’s design and development, for example, agile processes can involve iterative cycles and adjustments across the different phases outlined above. When it comes to deployment, operation and monitoring/evaluation typically occur in parallel. Moreover, in the case of adaptive systems, updating can occur continually during operation.

The volumes of data needed for ML systems and the complexity of technology supply chains mean that different activities across lifecycle phases are not always performed by actors within the same organisation. In contexts that involve third-party data providers, outsourcing different aspects of system design and development, or reliance on off-the-shelf tools, certain activities will be carried out by actors outside of the firm using the system.

Indeed, some of these activities might not be carried out by human actors, but by ML systems: recent innovations make it possible to automate large sections of an ML system’s development. However, in any of these cases, the structure of lifecycle phases remains unaffected by this, as the fundamental steps in designing, developing, and deploying an ML system stay the same.

## Exercises


**1**. Depending on the nature of a system, what kind of **validation** and **verification** can be used for **assessment**?

*Compare your answer with the solution below*

   ```{toggle}
    **empirical testing or formal verification**
   ```

**2**. In which **lifecycle phase** changes to the ML systems can be done? You have to choose one single answer.

       a. Validation and verification
       b. Business case and problem definition
       c. System retirement
       d. Monitoring and evaluation
       f. Integration

*Compare your answer with the solution below*

   ```{toggle}
    **c. System retirement**
   ```

**3**. The structure of the lifecycle phases are affected by the **automation** of large section of an ML system's development.

       a. True

       b. False
*Compare your answer with the solution below*

   ```{toggle}
    **b. False. The structure of the lifecycle phases should NOT be affected by the **automation** of large section of an ML system's development**
   ```

**4**. Lifecycle phases for **system deployment** occur **parallel**.

       a. True

       b. False
*Compare your answer with the solution below*

   ```{toggle}
    **a. True**
   ```
