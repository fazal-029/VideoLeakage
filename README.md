Federated learning (FL) allows multiple entities to
train a shared model collaboratively. Its core, privacy-preserving
principle is that participants only exchange model updates, such
as gradients, and never their raw, sensitive data. This approach
is fundamental for applications in domains where privacy and
confidentiality are important. However, the security of this very
mechanism is threatened by gradient inversion attacks, which
can reverse-engineer private training data directly from the
shared gradients, defeating the purpose of FL. While the impact
of these attacks is known for image, text, and tabular data,
their effect on video data remains an unexamined area of
research. This paper presents the first analysis of video data
leakage in FL using gradient inversion attacks. We evaluate
two common video classification approaches: one employing pre-
trained feature extractors and another that processes raw video
frames with simple transformations. Our initial results indicate
that the use of feature extractors offers greater resilience against
gradient inversion attacks.
We also demonstrate that image super-resolution techniques
can enhance the frames, extracted through gradient inversion attacks, 
enabling attackers to reconstruct higher-quality videos. 
Our experiments validate this across scenarios where the attacker has access to zero, one, or more reference frames from the target environment. 
We find that although feature extractors make attacks more challenging, leakage is still possible if the classifier lacks sufficient complexity. 
We, therefore, conclude that video data leakage in FL is a viable threat, and the conditions under which it occurs warrant further investigation.
