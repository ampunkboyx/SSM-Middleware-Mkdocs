<div class="col-md-12">

``` mermaid
graph LR
  subgraph System Integration Process Flow
    subgraph SSM Officer
        E-->F{Approve?}
    end
B--no-->C[Create Service Requestor/Agency Profile]
    subgraph Service Requestor/Agency
        A(Start)-->B{  Have a service requestor account?  }
        B--yes-->E[Subscribe Service]
        C-->D[/This is the text in the box/]
        D-->E[Subscribe Service]
        F--approve-->G[Perform Testing]
        G-->I{Tested Ok?}
        I--re-test-->I
        I-->Z[Production]
        Z-->J(End)
        F--reject-->H[Notify rejection of the subscription]
        H-->J
        style A fill:#008000,stroke:#333,stroke-width:4px
        style J fill:#008000,stroke:#333,stroke-width:4px
    end
  end
```
</div>