
# Microservices at Netflix and Other Companies

## 1) Netflix: Microservices Architecture
Netflix originally used a monolithic architecture where all features like streaming, recommendations, user management and many others were tightly bundled together. As the platform grew globally, this design struggled with slow deployments, limited scaling and outages. To solve this, Netflix broke its system into independent microservices. Each service like user authentification, recommendations, video streaming, billing runs separately and communicates over APIs. This allows teams to deploy code independently, scale specific functions and reduce system-wide failures. Netflix's microservice approach also uses tools like service discovery, circuit breakers and API gateways to manage service communication and failures.

**Key benefits Netflix gained:**
- Independent scaling of services
- Faster deployments and innovation
- Fault isolation where one service failing doesn't crash the whole system
- Increased resilience and global reliability since round 500+ microservices operate together to handle streaming traffic from billions of requests daily.

---

## 2) Two Other Companies Using Microservices

### eBay
eBay moved from a monolithic design into microservices to handle massive daily load, which includes billions of searches and database calls. By splitting functionality into smaller services, eBay improved developer productivity, enabled faster deployments and maintained stability even under heavy traffic.

### Spotify
Spotify also adopted microservices to support millions of music users across devices. The platform now runs hundreds of independent services, letting teams work autonomously, update services without affecting others and scale different parts like playlists or recommendations separately.

---

## 3) Companies That Moved from Microservices Back to Monolithic

Although microservices can be powerful, they are not always the best fit for every use case. In some scenarios, complexity, cost, latency and operational overhead can outweigh the benefits, leading companies to revert back to a monolithic architecture.

### Amazon Prime Video
Amazon's Prime Video team originally used a distributed microservices system for handling tasks such as video analysis and monitoring but over time they found that:
- Operating hundreds of microservices caused very high infrastructure costs
- Communication between services introduced latency
- Orchestration overhead made scaling inefficient

They consolidated important components into a monolithic application hence reducing costs by around 90% and simplifying deployment and maintenance.

### Segment
Segment which is a customer data platform moved from over 140 separate microservices back into a more unified architecture because the complexity and operational work became too heavy compared to the value.

---

## Summary

| Company | Architecture Used | Reason |
|---------|------------------|--------|
| Netflix | Microservices | Scalability, reliability, rapid innovation |
| eBay | Microservices | Handle heavy load, improve dev productivity |
| Spotify | Microservices | Support millions of users, scale features independently |
| Amazon Prime Video | Reverted to Monolith | Reduce cost, simplify system complexity |
| Segment | Reverted to Monolith | Manageability and reduced overhead |


*This therefore shows that microservices are excellent for large, complex systems needing independent scalability and frequent updates. But for some services like intense real-time processing a monolith can be simpler, cheaper and faster to maintain.*

# Work done by: ANSASIIRE NEHUM NAAMAYE S24B23\018


